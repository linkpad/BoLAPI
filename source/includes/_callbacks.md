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

## OnReset

* Called every draw reset.

``` lua
function OnReset()
    print("OnReset works")
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

## OnRecvChat

* Called when user send recv chat.

``` lua
function OnRecvChat(unit, text)
    print("OnRecvChat works - " .. unit.charName .. " wrote : " .. text)
end
```

## OnSendPacket

* Called when user send a packet

``` lua
function OnSendPacket(packet)
    print("OnSendPacket works")
end
```

## OnRecvPacket

* Called when user recv a packet

``` lua
function OnRecvPacket(packet)
    print("OnRecvPacket works")
end
```

## OnBugSplat

* Called when user bugsplat

``` lua
function OnBugSplat()
    
end
```

## OnAnimation

* Called when a unit does an animation

``` lua
function OnAnimation(unit, animation)
    print("OnAnimation works: Unit " .. unit.charName .. " did " .. animation)
end
```

## OnApplyParticle

* Called when a particle apply to a unit

``` lua
function OnApplyParticle(unit, particle)
    print("OnApplyParticle works: Unit " .. unit.charName .. " got " .. particle.charName)
end
```

## OnNotifyEvent

* Called on event

``` lua
function OnNotifyEvent(event, unit)
    print("OnNotifyEvent " .. unit.charName .. " -> " .. event)
end
```

## OnNewPath

* Called on new path

``` lua
function OnNewPath(unit, startPos, endPos, isDash, fSpeed, fGravity, fDistance)
    print("OnNewPath works")
end
```

## OnIssueOrder

* Called on IssueOrder

``` lua
function OnIssueOrder(unit, iAction, targetPos, Target)
    print("OnIssueOrder works")
end
```

## OnCastSpell

* Called on CastSpell

``` lua
function OnCastSpell(iSpell, startPos, endPos, Target)
    print("OnCastSpell works")
end
```

## OnApplyBuff

* Called on ApplyBuff

``` lua
function OnApplyBuff(Src, Target, Buff)
    print("OnApplyBuff works")
end
```

## OnUpdateBuff

* Called on UpdateBuff

``` lua
function OnUpdateBuff(Src, Buff, iStacks)
    print("OnUpdateBuff works")
end
```

## OnRemoveBuff

* Called on RemoveBuff

``` lua
function OnRemoveBuff(Src, Buff)
    print("OnRemoveBuff works")
end
```
