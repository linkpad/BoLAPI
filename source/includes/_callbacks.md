# CallBack Functions

## OnLoad

* Called when a script is loaded.

``` lua
function OnLoad()
    print("OnLoad works")
end
```

## OnUnload

* Called when a script is unloaded.

``` lua
function OnUnload()
    print("OnUnload works")
end
```

## OnDraw

* Called every draw tick.
* Should be use only for drawing purpose.

``` lua
function OnDraw()
    print("OnDraw works")
end
```

## OnTick

* Called every game tick.

``` lua
function OnTick()
    print("OnTick works")
end
```

## OnCreateObj

* Called when an object is created.

``` lua
function OnCreateObj(object)
    print("OnCreateObj works")
end
```

## OnDeleteObj

* Called when an object is deleted.

``` lua
function OnDeleteObj(object)
    print("OnDeleteObj works")
end
```

## OnWndMsg

* Called when the user use the mouse or the keyboard.

``` lua
function OnWndMsg(msg, key)
    print("OnWndMsg works")
end
```

## OnProcessSpell

* Called when a spell is casted.

``` lua
function OnProcessSpell(unit, spell)
    print("OnProcessSpell works")
end
```

## OnSendChat

* Called when user send text to the chat.

``` lua
function OnSendChat(text)
    print("OnSendChat works - user wrote : " .. text)
end
```