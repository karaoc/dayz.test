## Contents


- [BaseBuildingSettings](#BaseBuildingSettings)

- [BookSettings](#BookSettings)



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

# BookSettings

### "EnableBook"
Bool. If enabled, the book will be available to be opened. 

### "EnableStatusTab"
Bool. If enabled, the status tab will be available. The status tab contains character info like health, hunger/thirst values, etc. 

### "DisplayServerUptimeInStatusTab"
Bool. If enabled, server's current uptime will be displayed in the status tab. 

### "DisplayPlayerCountInStatusTab"
Bool. If enabled, displays current amount of players in the status tab. 

### "EnablePartyTab"
Bool. If enabled, the party tab will be available.

### "EnableServerInfoTab"
Bool. If enabled, the server info tab will be available.

### "EnableTerritoryTab"
Bool. If enabled, the territory tab will be available.

### "serverName"
String. Server name to be displayed in server info tab. 

### "infoTitle1"
String. Title to be displayed in server info tab. 

### "infoContent1"
String. Main body of the server info text in server info tab. 

### "infoTitle2"

### "infoContent2"

### "infoTitle3"

### "infoContent3"

### "ServerLogoPath"
Image set: image, for use in server info tab. 

### "WebsiteButton"
Bool. If enabled, the website button will be displayed in server info tab. 

### "WebsiteURL"
String. URL to open when website button is pressed. 

### "ForumsButton"
Bool. If enabled, the forums button will be displayed in server info tab. 

### "ForumsURL"
String. URL to open when forums button is pressed. 

### "DiscordButton"
Bool. If enabled, the Discord button will be displayed in server info tab. 

### "DiscordURL"
String. URL to open when Discord button is pressed. 
