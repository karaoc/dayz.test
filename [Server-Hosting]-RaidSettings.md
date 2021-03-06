Last updated the 24th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "ExplosionTime"
Integer. Time in seconds it takes for the ExpansionSatchel to explode.

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
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the wall, so 130. **Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, walls currently have an HP of 30,000.

### "CanRaidSafes"
Bool.
- 0 = Players won't be able to destroy Expansion safes.
- 1 = Allow to players to raid expansion safes.

### "SafeExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the safe, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. Less than 1 values work here as well, so 0x will disable damage to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

### "SafeProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the safe, so 130. **Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

### "BaseBuildingRaidMode"
Integrer.
- -1 = Expansion BaseBuilding elements can't be raided.
- 0 = every basebuilding elements can be raided.
- 1 = only doors/gates.
- 2 = only doors/gates/windows.

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/RaidSettings.json