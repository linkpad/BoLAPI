# Globals Functions


## IsKeyPressed

* Return true/false if key was pressed

`IsKeyPressed(key)`

``` lua
IsKeyPressed(string.byte("M"))
```

## IsKeyDown

* Return true/false if key is down

`IsKeyDown(key)`

``` lua
IsKeyDown(string.byte("M"))
```

## CastSpell

* Cast a spell

Uses Spell or Item :

`CastSpell(iSpell)`

Uses Spell or Item at position :

`CastSpell(iSpell, x, z)`

Uses Spell or Item at Target Position :

`CastSpell(iSpell, target)`

## LevelSpell

* Level Up a Spell

`LevelSpell(iSpell)`

## print

* Print text to chat (local only)

`print(text)`

## PrintChat

* Print text to chat (local only)

`PrintChat(text)`

## SendChat

* Send Chat (external chat, "/" not handled)

`SendChat(text)`

## BlockChat

* Block last chat message.

`BlockChat()`

## DrawText

* Draw Text over screen

`DrawText(text, size, x, y, ARGB)`

``` lua
function OnDraw()
    DrawText("this is a draw text", 12, 10, 10, ARGB(255,255,255,255))
end
```

## DrawLine

* Draw Line over screen

`DrawLine(startX, startY, endX, endY, size, ARGB)`

``` lua
function OnDraw()
    DrawLine(10, 10, 50, 10, 2, ARGB(255,255,255,255))
end
```

## DrawRectangle

* Draw Rectangle over screen

`DrawRectangle(x, y, width, height, ARGB)`

``` lua
function OnDraw()
    DrawRectangle(10, 10, 50, 10, ARGB(255,255,255,255))
end
```

## DrawCircle

* Draw a circle around game object

`DrawCircle(x, y, z, size, RGB)`

## DrawRectangleOutline

`DrawRectangleOutline(x, y, width, height, color, borderWidth)`

## DrawLineBorder3D

`DrawLineBorder3D(x1, y1, z1, x2, y2, z2, size, color, width)`

## DrawLineBorder

`DrawLineBorder(x1, y1, x2, y2, size, color, width)`

## DrawCircleMinimap

`DrawCircleMinimap(x, y, z, radius, width, color, quality)`

## DrawCircle2D

`DrawCircle2D(x, y, radius, width, color, quality)`

## DrawCircle3D

`DrawCircle3D(x, y, z, radius, width, color, quality)`

## DrawLine3D

`DrawLine3D(x1, y1, z1, x2, y2, z2, width, color)`

## DrawLines3D

`DrawLines3D(points, width, color)`

## DrawTextA

`DrawTextA(text, size, x, y, color, halign, valign)`

## DrawText3D

`(text, x, y, z, size, color, center)`

## GetMyHero

* Return your Player as unit

`GetMyHero()`

## GetTarget

* Return your target as unit (or nil if none)

`GetTarget()`

## GetTickCount

* Return current tick

`GetTickCount()`

## GetLatency

* Return latency

`GetLatency()`

## GetCursorPos

* Return cursor position on the screen

`GetCursorPos()`

## GetDistanceSqr

* Return the distance^2

`GetDistanceSqr(p1, p2)`

<aside class="notice">Faster than <code>GetDistance(p1, p2)</code> for comparison of distances</aside>

## GetDistance

* Return the distance

`GetDistance(p1, p2)`

## GetEnemyHeroes

* Return all enemy heroes in a table

`GetEnemyHeroes()`

## GetAllyHeroes

* Return all ally heroes in a table

`GetAllyHeroes()`

## GetSave

* used to save data between matches. It can save all data except userdata, even functions !

`GetSave(name)`

``` lua
	GetSave("mySave").print = print
	--> nextGame (Or reload)
	GetSave("mySave").print("Hello")
```

## CreateDirectory

* Create a directory and return true or false, only works if the folder doesn't already exist

`CreateDirectory(path)`

## DirectoryExist

* Check if a directory exist and return true or false

`DirectoryExist(path)`

## ReadFile

* Return text of a file

`ReadFile(path)`

## WriteFile

* Return true if could write to file; mode is optional

`WriteFile(text, path, mode)`

## FileExist

* Return true if file exists

`FileExist(path)`

## DeleteFile

* Return true if file is succesfully deleted

`DeleteFile(path)`

## GetFileSize

* Return the size of a file

`GetFileSize(path)`

## DelayAction

* Delays a function call
- Delay is in seconds

`DelayAction(func, delay, args)`

## EnableOverlay

* Enable overlay

`EnableOverlay()`

## DisableOverlay

* Disable overlay

`DisableOverlay()`

## CursorIsUnder

* return if cursor is under a rectangle

`CursorIsUnder(x, y, sizeX, sizeY)`

## createSprite

* Create a sprite object 
* Files are loaded from "Sprites" folder

`createSprite(file)`

## UpdateWindow

* updates WINDOW_[X/Y/W/H]

`UpdateWindow()`

## D3DXVECTOR3

* Create a D3DXVECTOR3 object 
* 
`D3DXVECTOR3(x, y, z)`

## WorldToScreen

* Return screen position based on ingame coordinates

`WorldToScreen(D3DXVECTOR3)`

## ValidTarget

* Return true if the target is valid

`ValidTarget(object, distance, enemyTeam)`

## BuffIsValid

* Return true if the buff is valid

`BuffIsValid(buff)`

## TargetHaveBuff

* Return if target have buff

`TargetHaveBuff(buffName, target)`

## CountEnemyHeroInRange

* return number of enemy in range
* object is optional

`CountEnemyHeroInRange(range, object)`

