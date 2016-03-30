# Unit Members

## unit.name

* Return the unit name

## unit.charName

* Return the unit character name

## unit.level

* Return the unit level (only for hero)

## unit.visible

* Return true/false if the unit is visible

## unit.type

* Return the unit type

## unit.x

* Return the x position of the unit

## unit.y

* Return the y position of the unit

## unit.z

* Return the z position of the unit

## unit.isAI

* Return true/false if unit is AI

## unit.isMe

* Return true/false if unit is my hero

## unit.buffCount

* Return unit buffCount

## unit.totalDamage

* Return unit totalDamage

## unit.dead

* Return true/false if unit is dead

## unit.team

* Return the unit team

## unit.networkID

* Return the unit networkID

## unit.health

* Return the current health of the unit

## unit.maxHealth

* Return the max health of the unit

## unit.mana

* Return the current mana of the unit

## unit.maxMana

* Return the max mana of the unit

## unit.bInvulnerable
## unit.bPhysImune
## unit.bMagicImune
## unit.bTargetable
## unit.bTargetableToTeam
## unit.controlled
## unit.cdr
## unit.critChance
## unit.critDmg
## unit.hpPool
## unit.hpRegen
## unit.mpRegen
## unit.attackSpeed
## unit.expBonus
## unit.hardness
## unit.lifeSteal
## unit.spellVamp
## unit.physReduction
## unit.magicReduction
## unit.armorPen
## unit.magicPen
## unit.armorPenPercent
## unit.magicPenPerecent
## unit.addDamage
## unit.ap
## unit.damage
## unit.armor
## unit.magicArmor
## unit.ms
## unit.range
## unit.gold
## unit.pos
## unit.minBBox
## unit.maxBBox
## unit.armorMaterial
## unit.weaponMaterial
## unit.deathTimer
## unit.canAttack
## unit.canMove
## unit.isStealthed
## unit.isRevealSpecificUnit
## unit.isTaunted
## unit.isCharmed
## unit.isFeared
## unit.isAsleep
## unit.isNearSight
## unit.isGhosted
## unit.isNoRender
## unit.isFleeing
## unit.isForceRenderParticles

# Unit Methods

* Only for Hero

## unit:HoldPosition

* The unit hold the current position

`unit:HoldPosition()`

## unit:MoveTo

* The unit move to the X and Z position.

`unit:MoveTo(x, z)`

## unit:Attack

* The unit attack the specified target

`unit:Attack(target)`

## unit:GetDistance

* Get the distance from the unit to the target

`unit:GetDistance(target)`

## unit:CalcDamage

* Calculate the damage that can be dealt to the target

`unit:CalcDamage(target, maxDamage)`

## unit:CalcMagicDamage

* Calculate the magic damage that can be dealt to the target

`unit:CalcMagicDamage(target, maxMagicDamage)`

## unit:getBuff

* Return buff object of the specified index

`unit:getBuff(index)`

## unit:getInventorySlot

* Return item ID of the specified slot
* Slot are from ITEM_1 to ITEM_6

`unit:getInventorySlot(slot)`

## unit:getItem

* Return LoLItem
* Slot are from ITEM_1 to ITEM_6

`unit:getItem(slot)`

## unit:GetSpellData

* Return Spell object

`unit:GetSpellData(iSpell)`


## unit:CanUseSpell

* Return Spell State

`unit:CanUseSpell(iSpell)`
