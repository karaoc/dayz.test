Last updated the 19th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "PlayerLocationNotifier"
Bool.
- 0 = The player will not get any notifications telling him where he is and what time is it.
- 1 = The player will get a dayz mod styled notification with the town name and time and date.

### "EnableGlobalChat"
Bool.
- 0 = The global chat (blue chat) will be disabled.
- 1 = It will enable the global chat. The global chat allow players to talk to anyone from anywhere on the map.

### "EnableGravecross"
Bool.
- 0 = Gravecross will be disabled. The dead player inventory will stay on him.
- 1 = Gravecross will be enabled. When a player will die a Gravecross will spawn on him with all his stuff in it. This is usualy used to prevent body despawn between restarts.

### "GravecrossDeleteBody"
Bool. Only work if "EnableGravecross" is enabled.
- 0 = If you still want the deadbody next to the Gravecross because you want your players to skin deadplayers.
- 1 = This will delete the body of the dead player. Why use this ? To only have the Gravecross and not have a naked deadbody next to it.

### "GravecrossTimeThreshold"
Integrer. Only work if "EnableGravecross" is enabled.
- How long the Gravecross will stay before it despawn.

### "UseCustomMappingModule"
Bool. **WARNING** custom mapping have a big impact on server and player performance.
- 0 = The expansion custom mapping will be disabled, this will not disable custom interiors or ivy.
- 1 = The expansion custom mapping will be enabled, roadblocks, forests, new buildings and more detailed roads will be added. Currently, only ChernarusPlus have custom mapping.

### "Mapping"
Array. List all the locations with custom mapping made by the mod Expansion. If you want to remove a location, just remove the line !

### "ObjectsToDelete"
Array. You can indicate the position and the name of a specific mapped object to be removed. This action can be done to multiple objects.

### "InteriorBuilding"
Bool. Have a huge impact on server and player performance !
- 0 = Interiors won't be filled with new props.
- 1 = Interiors will be more detailled.

### "Ivies"
Bool. Only work for ChernarusPlus !
- 0 = No custom ivies will be added to the map
- 1 = Custom Ivies in specific locations will be added to the map.

### "EnableLamps"
Integer.
- 0 = Disabled - The streets lights are off;
- 1 = Generators - Currently unused. Would require you to fix a generator to make street lights work. - **CURRENTLY DOESNT WORK**
- 2 = Always On - Street lights are emitting lights but some of them will stay off intentionnaly.
- 3 = Always On (Everywhere) - Force every lights to be turned on;

### "EnableGenerators" - **CURRENTLY DOESNT WORK**
Bool. Currently unused 
- 0 = No generators will be spawned insithe towns and villages.
- 1 = Will spawn in towns and villages generators for the mode 1 for "EnableLamps".

### "EnableLighthouses"
Bool.
- 0 = the lighthouses won't emit a light beam.
- 1 = turns on the light of every lighthouses of the map.

### "EnableHUDNightvisionOverlay"
Bool.
- 0 = Use the NVG vanilla overlay (in short a green screen)
- 1 = Add a immersive NVG overlay

### "DisableMagicCrosshair"
Bool. 
- 0 = Will use the current DayZ vanilla aiming system.
- 1 = enable DayZ Alpha style for the cursor. This setting is needed for the laser sight attachement to be accurate.

### "EnablePlayerTags"
Bool.
- 0 = This feature will be disabled. If you are a RolePlay server you might want to turn this off.
- 1 = When looking at a player, a "player tag" will be visible. This player tag concist of a icon and the name of the player.

### "PlayerTagViewRange"
Integer. The distance requiried to see the player tag. The value is in meters, in other words 5 is 5 meters.

### "EnablePlayerList"
Bool.
- 0 = This feature will be turned off.
- 1 = Allow players to see a player list of the online players.

### "EnableAutoRun"
Bool.
- 0 = This feature will be turned off.
- 1 = Allow the player to use the autorun feature. It will still work when they will be in their inventory.
  - SHIFT + Z = Auto Sprint
  - CTRL + Z = Auto Walk
  - Z = Auto Jog

### "UnlimitedStamina"
Bool.
- 0 = Vanilla staminae
- 1 = The stamina will be unlimited but still balanced (aiming, heavy attacks and so on).

### "UseDeathScreen"
Bool.
- 0 = Deathscreen will be a blackscreen as usual. Vanilla way
- 1 = Add back the old school deathscreen (with the bloody hand).

### "UseDeathScreenStatistics"
Bool.
- 0 = You won't be able to know your stats when dead like in vanilla.
- 1 = When dead you will be able to know your personal stats.

### "UseNewsFeedInGameMenu"
Bool.
- 0 = The news feed in the pause menu will be removed
- 1 = The news feed in the pause menu will be enabled

# Raw file

    {
        "PlayerLocationNotifier": 1,
        "EnableGlobalChat": 1,
        "EnablePartyChat": 1,
        "EnableTransportChat": 1,
        "EnableGravecross": 0,
        "GravecrossDeleteBody": 1,
        "GravecrossTimeThreshold": 1200,
        "Mapping": {
            "UseCustomMappingModule": 1,
            "Mapping": [],
            "ObjectsToDelete": [],
            "BuildingInteriors": 1,
            "BuildingIvys": 1
        },
        "EnableLamps": 3,
        "EnableGenerators": 0,
        "EnableLighthouses": 1,
        "EnableHUDNightvisionOverlay": 1,
        "DisableMagicCrosshair": 1,
        "EnablePlayerTags": 1,
        "PlayerTagViewRange": 5,
        "EnablePlayerList": 1,
        "EnableAutoRun": 1,
        "UnlimitedStamina": 0,
        "UseDeathScreen": 1,
        "UseDeathScreenStatistics": 1,
        "UseNewsFeedInGameMenu": 1
    }