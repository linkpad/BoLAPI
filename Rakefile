require 'middleman-gh-pages'
require 'tmpdir'

desc 'Generate site from Travis CI and publish site to GitHub Pages'
task :travis do
  # If this is a pull request, do a simple build and stop
  if ENV['TRAVIS_PULL_REQUEST'].to_s.to_i > 0
    puts 'Pull request detected. Executing build only.'
    sh 'bundle exec rake build'
    next
  end

  # Set repo, branch, and commit revision for later use
  repo = `git config remote.origin.url`.gsub(/^git:/, 'https:').strip
  branch = repo =~ /github\.com\.git$/ ? 'master' : 'gh-pages'
  rev = `git rev-parse HEAD`.strip[0..6]

  # Build the project and set build location
  sh 'bundle exec rake build'
  origin = "#{Dir.getwd}/build"

  # Make temporary directory an copy files
  Dir.mktmpdir do |dir|
    Dir.chdir dir do
      fail "Deployment failed." unless Dir.exists? origin
      sh "git clone --branch #{branch} #{repo} ."
      sh %(rsync -rt --del --exclude=".git" "#{origin}/" .)

      # Setup credentials so Travis CI can push to GitHub
      verbose false do
        sh "git remote set-url --push origin #{repo}"
        sh "git remote set-branches --add origin #{branch}"
        sh "git config user.name Travis"
        sh "git config user.email travis@travis-ci.org"
        sh 'git config credential.helper "store --file=.git/credentials"'
        File.open('.git/credentials', 'w') do |f|
          f << "https://#{ENV['GITHUB_TOKEN']}:@github.com"
        end
      end

      # Add files, create commit, and push to GitHub
      sh 'git add --all'
      sh "git commit -m 'Built from https://github.com/#{ENV['TRAVIS_REPO_SLUG']}/commit/#{rev}'"
      verbose false do
        sh "git push -q #{repo} #{branch}"
      end

      File.delete '.git/credentials'
    end
  end
end
