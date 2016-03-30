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


## createSprite

* Create a sprite object 
* Files are loaded from "Sprites" folder

`createSprite(file)`

## UpdateWindow

* updates WINDOW_[X/Y/W/H]

`UpdateWindow()`
