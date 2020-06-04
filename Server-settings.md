## Contents


- 1. [BaseBuilding](#BaseBuildingSettings)



# BaseBuildingSettings
### "CanCraftVanillaBasebuilding"
Bool. If set to 0, you can not craft vanilla basebuilding objects (FenceKit and WatchTowerKit). If 1, you can. 

### "CanCraftExpansionBasebuilding"
Bool. If set to 0, you can not craft DayZ Expansion Basebuilding objects. 

### "CanRaidSafes"
Bool. If set to 0, when a safe is ruined, nothing happens. If set to 1, it will unlock and open. 

"ExplosionTime"
Integer. Time in seconds it takes for a ExpansionExplosiveBase to countdown and detonate. 

### "ExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the wall, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. **Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. 
Note, walls currently have an HP of 30,000. 

### "ProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the wall, so 130.** Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. 
Note, walls currently have an HP of 30,000. 

### "TerritoryMode"
Integer. Two modes currently:
0: You can build anywhere even if you do not have a territory, but if you do build one, nobody else can build inside it. 
1: You can not build unless you have a territory

### "CodeLockLength"
Integer. The length of passwords you can put into your code locks. 