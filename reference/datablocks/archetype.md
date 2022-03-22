---
description: GameData_ArchetypeDataBlock_bin.json
---

# ArchetypeDataBlock

No description provided.

***

## Fields

### PublicName - [LocalizedText](../nested-types/localizedtext.md) (nested type)

The displayed name for a weapon in-game.

### Description - [LocalizedText](../nested-types/localizedtext.md) (nested type)

The description displayed in-game when selecting a weapon.

### FireMode - [eWeaponFireMode](../enum-types.md#eweaponfiremode) (enum)

The firing mode for a weapon. Semi-automatic, Burst Fire, Full Auto, and Semi-Burst.

### RecoilDataID - UInt32

Pulls a peristent ID from RecoilData to set the weapon's recoil settings.

### DamageBoosterEffect - [AgentModifier](../enum-types.md#agentmodifier) (enum)

Determines which persistent ID from BoosterImplantTemplateData will affect this weapon. Not recommended to use.

### Damage - Single

The damage value of each bullet or pellet this weapon deals.

### DamageFalloff - Vector2

The minimum range before the weapon starts to deal reduced damage, and the max range before 10% damage is dealt. All weapons stop dealing damage at 100 meters.

### StaggerDamageMulti - Single

A multiplier on the Damage value to raise or lower how much the weapon staggers enemies.

### PrecisionDamageMulti - Single

A multiplier on the Damage value to raise or lower how much headshot / weakspot damage the weapon deals.

### DefaultClipSize - Int32

The mag size of a weapon. The mag part used may affect this value.

### DefaultReloadTime - Single

The amount of time it takes to reload a weapon. The front part or stock part used may affect this value.

### CostOfBullet - Single

The value of each bullet. The max value a weapon has is determined by AmmoStandardMaxCap, AmmoSpecialMaxCap and AmmoClassMaxCap. MaxCap/CostOfBullet = Stock/Reserve Ammo.

### ShotDelay - Single

The time in seconds between each shot.

### PiercingBullets - Boolean

Determines if the weapon's bullets will pierce. Shotguns and sentries can not pierce without the use of a plugin.

### PiercingDamageCountLimit - Int32

Determines how many enemies can be hit by a single bullet. Hard capped at 5. Ex: setting this value to 3 means 1 bullet can hit 3 enemies.

### HipFireSpread - Single

Determines how much a weapon's shots will spread while not aiming down sights. Does not apply to shotguns.

### AimSpread - Single

Determines how much a weapon's shots will spread while aiming down sights. Does not apply to shotguns.

### EquipTransitionTime - Single

Determines how long in seconds it takes for a weapon to fully equip. Does not affect how long it takes to begin shooting when equipping.

### EquipSequence - [List WeaponAnimSequenceItem](../nested-types/weaponanimsequenceitem.md) (nested type)

Determines the equip animation.

### AimTransitionTime - Single

Determines how long in seconds it takes for a weapon to fully aim down sights. Does not impact or delay firing.

### AimSequence - [List WeaponAnimSequenceItem](../nested-types/weaponanimsequenceitem.md) (nested type)

Determins the ADS animation.

### BurstDelay - Single

Delay between each burst if the weapon uses the Burst Fire mode.

### BurstShotCount - Int32

Determines how many shots are fired in a single burst.

### ShotgunBulletCount - Int32

Determines how many pellets a shotgun will fire per bullet.

### ShotgunConeSize - Int32

Determines the general spread of shotgun pellets.

### ShotgunBulletSpread - Int32

Changes the spread pattern and spacing between bullets.

### SpecialChargetupTime - Single

Determines how long the firing button must be held before the gun fires.

### SpecialCooldownTime - Single

No description proviided.

### SpecialSemiBurstCountTimeout - Single

No description provided.

### Sentry_StartFireDelay - Single

Determines how long the sentry waits before firing when it acquires a target.

### Sentry_RotationSpeed - Single

Determines how fast a sentry can rotate to track a target.

### Sentry_DetectionMaxRange - Single

Determines the max range a sentry can lock onto a target.

### Sentry_DetectionMaxAngle - Single

Determines the max turning angle left or right a sentry can lock onto a target. 180 degrees will allow the sentry to fire in all directions.

### Sentry_FireTowardsTargetInsteadOfForward - Boolean

Gives the sentry very high accuracy when enabled.

### Sentry_LongRangeThreshold - Single

Determines how far an enemy must be before enabling the Sentry Gun Long Range Damage booster effect.

### Sentry_ShortRangeThreshold - Single

Determines how far an enemy can be before disabling the Sentry Gun Short Range Damage booster effect.

### Sentry_LegacyEnemyDetection - Boolean

Gives the sentry the old detection. Not recommended as it causes poor tracking.

### Sentry_FireTagOnly - Boolean

Determines if the sentry requires Bio-Tracker pings to target enemies.

### Sentry_PrioTag - Boolean

Determines if the sentry should target enemies with Bio-Tracker pings before others.

### Sentry_StartFireDelayTagMulti - Single

Multiplier for the StartFireDelay value when locked on to a Bio-Tracked enemy.

### Sentry_RotationSpeedTagMulti - Single

Multiplier for the RotationSpeed value when locked on to a Bio-Tracked enemy.

### Sentry_DamageTagMulti - Single

Multiplier for the Damage value when locked on to a Bio-Tracked enemy.

### Sentry_StaggerDamageTagMulti - Single

Multiplier for the Stagger value when locked on to a Bio-Tracked enemy.

### Sentry_CostOfBulletTagMulti - Single

Multiplier for the CostOfBullet value when locked on to a Bio-Tracked enemy.

### Sentry_ShotDelayTagMulti - Single

Multiplier for the ShotDelay value when locked on to a Bio-Tracked enemy.
