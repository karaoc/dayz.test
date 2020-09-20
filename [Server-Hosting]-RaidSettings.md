Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "ExplosionTime"
Integer. Time in seconds it takes for a ExpansionExplosiveBase to countdown and detonate.

### "ExplosiveDamageWhitelist"
Array of string. Put every classname of the explosive items you want to be able to be used for raiding.

The classnames are not the **weapons items** nor the **explosives items** but the explosion itself. For example you can disable rpg explosions with "Expansion_RPG_Explosion"

        "ExplosiveDamageWhitelist": [
            "classname02_withaCommaAtTheEnd",
            "classname03_withoutCommaAtTheEndBecauseItsTheLastOne"
        ],

### "EnableExplosiveWhitelist"
Bool.
- 0 = Every items from the game will be able to raid basebuilding elements regardless of ExplosiveDamageWhitelist.
- 1 = Only the items listed above will be able to raid basebuilding elements.

### "ExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the wall, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. Less than 1 values work here as well, so 0x will disable damage to base parts, and .5x will halve them. Note, walls currently have an HP of 30,000.

### "ProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the wall, so 130.** Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, walls currently have an HP of 30,000.

### "CanRaidSafes"
Bool. If set to 1, allow to players to raid expansion safes.
- 0 = Will not do what 1 do and instead do nothing.
- 1 = Every vehicles on the map will have a marker displayed on the map on their position.

### "SafeExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the safe, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. Less than 1 values work here as well, so 0x will disable damage to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

### "SafeProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the safe, so 130.** Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

# Raw file

    {
        "ExplosionTime": 30,
        "ExplosiveDamageWhitelist": [
            "Expansion_C4_Explosion",
            "Expansion_RPG_Explosion"
        ],
        "EnableExplosiveWhitelist": 0,
        "ExplosionDamageMultiplier": 50,
        "ProjectileDamageMultiplier": 1,
        "CanRaidSafes": 1,
        "SafeExplosionDamageMultiplier": 17,
        "SafeProjectileDamageMultiplier": 1
    }
