![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/commits/master/ServerProfile/ExpansionMod/Settings) to see the server settings files
* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/commit/befd7e7cfee6a85f4cc1b26326e5d6c6a4b11ed7) to see the lastest changes for server settings

### WARNING! The lastest expansion update (1.01) tweaked/added the follwoing :

#### TerritorySettings
- "MaxInTerritory" became "MaxMembersInTerritory" (this is not new but just in case you are not aware that have been changed in the past updates)

#### PartySettings
- **added** bool "EnableQuickMarker"

#### BuildingSettings
- **added** float SafeExplosionDamageMultiplier
- **added** float SafeProjectileDamageMultiplier
- **added** bool CanDismantleFlag


***


## Contents


- [BaseBuildingSettings](#BaseBuildingSettings)

- [BookSettings](#BookSettings)

- [GeneralSettings](#GeneralSettings)

- [MapSettings](#MapSettings) (last one TODO)

- [MissionSettings](#MissionSettings) (last one TODO)

- [PartySettings](#PartySettings)

- [SafeZoneSettings](#SafeZoneSettings) (last two TODO)

- [SpawnSettings](#SpawnSettings)

- [TerritorySettings](#TerritorySettings)



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

### "AllowedItemsToPlaceEveryWhereButNotInEnemyTerritory"
Array of string. Only used if TerritoryMode is set to 1.
Put every classname of the item, you want to be able to be placed outside of the territory.

### "AllowedItemsToPlaceInEnemyTerritory"
Array of string.
Put every classname of the item, you want to be able to be placed in the territory where you are not a member of him.

### "DoDamageWhenEnterWrongCodeLock"
Bool. If set to 0, the player will not take damage if he enters a wrong code lock. If set to 1, he will take damage.

### "DamageWhenEnterWrongCodeLock"
Float. The number of damage the player will take when he types a wrong code lock.

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
String. Title to be displayed in server info tab. 

### "infoContent2"
String. Main body of the server info text in server info tab. 

### "infoTitle3"
String. Title to be displayed in server info tab. 

### "infoContent3"
String. Main body of the server info text in server info tab. 

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

# GeneralSettings
### "PlayerLocationNotifier"
Bool. When enabled, show to the player the name of the city he just got into and time of day

### "ShowPlayerJoinServer"
Bool. When enabled, notify the player who joined or left the server.

### "JoinMessageType"
Integer.
0. Will display the player joined message in the globalchat
1. Will display the player joined message in a notification

### "LeftMessageType"
Integer.
0. Will display the player left message in the globalchat
1. Will display the player left message in a notification

### "EnableKillFeed"
Bool. When enabled, notify the player of whom got killed and how.

### "KillFeedMessageType"
Integer.
0.  Will display the killfeed message in the globalchat
1.  Will display the killfeed message in a notification

### "EnableHumanity"
Bool. This feature currentmy does nothing. 

### "UseCustomMappingModule"
Bool. When enabled, add custom mapping. Have a huge impact on server performance !

### "Mapping"
Array. List all the locations with custom mapping. 

### "InteriorBuilding"
Bool. When enabled, add more detailed interiors. Have a huge impact on server performance !

### "Ivies"
Bool. When enabled, allow ivies to be on some building. Only work for Chernarus !

### "LightingConfig"
Integer.

1. : Default - Default lighting of dayz we all know.
2. : Dark - Make the night very dark, the day is with default lighting.
3. : Gloom - Change how lighting work for night and day. The night is a bit darker than default but not as much as Dark mode. The day is more "gloomy", everything shines more !

### "EnableLamps"
Integer.

0. Disabled - The streets lights are off;
1. Generators - Currently unused. Would require you to fix a generator to make street lights work.
2. Always On - Street lights are emitting lights but some of them will stay off intentionnaly.
3. Always On (Everywhere) - Force every lights to be turned on;

### "EnableGenerators"
Bool. Currently unused, will spawn town/village generators for the mode 1 for "EnableLamps"

### "EnableLighthouses"
Bool. If enabled, turns on the light of every lighthouses of the map.

### "EnableAutoRun"
Bool. If enabled, allow the player to autojog.

### "NeedGPSItemForKeyBinding"
Bool. If enabled, require the player to have the GPS item in his inventory to open the GPS

### "NeedMapItemForKeyBinding"
Bool. If enabled, require the player to have the map item in his inventory to open the map

### "EnableHUDNightvisionOverlay"
Bool. If enabled, add a immersive NVG overlay

### "EnablePlayerTags"
Bool. If enabled, show the player tag when your cursor is on him.

### "PlayerTagViewRange"
Integer. Distance requiried to see the tag. The value is in meter, in other words 5 is 5 meters.

### "EnableHumanityOnPlayerTags"
Bool. If enabled, show the player tag Humanity when your cursor is on him.

### "EnablePlayerList"
Bool. If enabled, allow players to see the player list.

### "UnlimitedStamina"
Bool. If enabled, make stamina unlimited.

### "SpawnVehicleWithRandomSkin"
Bool. If enabled, make vehicles spawn with random skins.

### "VehicleSync"
Integer. Currently unused.

# MapSettings
### "EnableMap"
Bool. If enabled, 

### "UseMapOnMapItem"
Bool. If enabled, the default map used for the map item when used will be expansion map.

### "CanCreateMarker"
Bool. If enabled, allow the player to create markers.

### "ShowPlayerPosition"
Bool. If enabled, show the player position on the map.

### "CanCreatePartyMarkers"
Bool. If enabled, allow the player to create party markers.

### "ShowMapStats"
Bool. If enabled, TODO

### "CanCreate3DMarker"
Bool. If enabled, allow the player to create 3D markers.

### "ShowPartyMembersMapMarkers"
Bool. If enabled, show the player teammates position on the map.

### "DistanceForPartyMarkers"
Integrer. Distance in meters before the 3d marker fade out. Could not go over bubble network distance ~1000 m per default in DayZ

### "ShowServerMarkers"
Bool. If enabled, show server map markers.

### "CanOpenMapWithKeyBinding"
Bool. If enabled, the player can open the map with a keybind instead of interacting with th physical map

### "ServerMarkers"
Array. Allow server owners to display server markers on the map.
**TODO**

# MissionSettings
### "Enabled"
Bool. If enabled, activate missions.

### "TimeBetweenMissions"
Integrer. Time in milliseconds before a new mission start

### "MinMissions"
Integrer. Minimum mission allowed at once.

### "MaxMissions"
Integrer. Maximum mission allowed at once.

### "Missions" TODO
Array.

# PartySettings
### "EnableParties"
Bool. If enabled, allow players to create parties.

### "MaxInParty"
Integrer. Maximum of players allowed in a single party. If <= 0, unlimited party size.

### "ShowPartyMembers3DMarkers"
Bool. If enabled, show a 3d marker above the head of your teammates.

### "UseWholeMapForInviteList"
Bool. If enabled, you can invite everyone from anywhere regardless of the distance.

### "EnableQuickMarker"
Bool. If enabled allow players to use QuickMarkers (act like a ping ingame).

# SafeZoneSettings
### "Enabled"
Bool. Enable Safezone when set to 1.

### "EnableVehicleinvincibleInsideSafeZone"
Bool. When enabled, Vehicle damage is disabled.

### "FrameRateCheckSafeZoneInMs"
Integrer. How often in ms the server need to check if the player is inside a Safezone.

### "CircleZones"
Array. 
- Type: **TODO**
- Center: where the zone should be on the map
- Radius: Size of the zone

### "PolygonZones"
Array.
- Type: **TODO**
- Positions: **TODO**
- CenterPolygon: where the zone should be on the map
- RadiusPolygon: Size of the zone

# SpawnSettings
### "UseStartingGear"
Bool. If enabled, will use the starting gear configured in this file

### "UsingUpperGear"
Bool. If enabled, use the upper gear configured

### "UsingPantsGear"
Bool. If enabled, use the pants gear configured

### "UsingBackpackGear"
Bool. If enabled, use the backpack gear configured

### "SpawnBackpacks"
Array. list of classnames used for the items spawning inside the backpack

### "UpperGear"
Array. list of classnames used for the upper gear

### "PantsGear"
Array. list of classnames used for the pants gear

### "BackpackGear"
Array. list of classnames used for the backpack gear

# TerritorySettings
### "EnableTerritories"
Bool. If enabled, use the expansion territory system

### "UseWholeMapForInviteList"
Bool. If enabled, will make the whole map available in invite list, instead only nearby players.

### "TerritorySize"
Float. the radius of territory in meters.

### "MaxMembersInTerritory"
Integer. The max amount of members allowed per territories. If <= 0, unlimited territory size.

### "MaxTerritoryPerPlayer"
Integer. The max amount of territories allowed per player. If <= 0, unlimited territory allowed.