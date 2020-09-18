Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "PlayerLocationNotifier"
Bool. When enabled, show to the player the name of the city he just got into and time of day
- 0 = 
- 1 = 

### "EnableGlobalChat"
Bool. If set to 1, will enable global chat. The global chat allow players to talk to anyone from anywhere on the chat.
- 0 = 
- 1 = 

### "EnableGravecross"
Bool. If set to 1, will enable Gravecross. When a player will die a grave will spawn on him with all his stuff on it. This is usualy used to prevent body despawn between restarts.
- 0 = 
- 1 = 

### "GravecrossDeleteBody"
Bool. If set to 1, will delete the body of the dead player. Only work if "EnableGravecross" is enabled.
- 0 = 
- 1 = 

### "GravecrossTimeThreshold"
Integrer. Documentation todo

### "UseCustomMappingModule"
Bool. if set to 1, add custom mapping. Have a huge impact on server performance !
- 0 = 
- 1 = 

### "Mapping"
Array. List all the locations with custom mapping. 

### "ObjectsToDelete"
Array. You can indicate the position and the name of a specific mapped object to be removed. This action can be done to multiple objects.

### "InteriorBuilding"
Bool. if set to 1, add more detailed interiors. Have a huge impact on server performance !
- 0 = 
- 1 = 

### "Ivies"
Bool. if set to 1, allow ivies to be on some building. Only work for Chernarus !
- 0 = 
- 1 = 

### "EnableLamps"
Integer.
- 0 = Disabled - The streets lights are off;
- 1 = Generators - Currently unused. Would require you to fix a generator to make street lights work. - CURRENTLY DOESNT WORK
- 2 = Always On - Street lights are emitting lights but some of them will stay off intentionnaly.
- 3 = Always On (Everywhere) - Force every lights to be turned on;

### "EnableGenerators" - **CURRENTLY DOESNT WORK**
Bool. Currently unused, will spawn town/village generators for the mode 1 for "EnableLamps"
- 0 = 
- 1 = 

### "EnableLighthouses"
Bool. If set to 1, turns on the light of every lighthouses of the map.
- 0 = 
- 1 = 

### "EnableHUDNightvisionOverlay"
Bool. If set to 1, add a immersive NVG overlay
- 0 = 
- 1 = 

### "DisableMagicCrosshair"
Bool. If set to 1, enable DayZ Alpha style for the cursor. This setting is needed for the laser sight attachement to be accurate.
- 0 = 
- 1 = 

### "EnablePlayerTags"
Bool. If set to 1, show the player tag when your cursor is on him.
- 0 = 
- 1 = 

### "PlayerTagViewRange"
Integer. Distance requiried to see the tag. The value is in meter, in other words 5 is 5 meters.
- 0 = 
- 1 = 

### "EnablePlayerList"
Bool. If set to 1, allow players to see the player list.
- 0 = 
- 1 = 

### "EnableAutoRun"
Bool. If set to 1, allow the player to use the autorun feature.
- 0 = 
- 1 = 

### "UnlimitedStamina"
Bool. If set to 1, the stamina will be unlimited.
- 0 = 
- 1 = 

### "UseDeathScreen"
Bool. If set to 1, enable the old school deathscreen (with the bloody hand).
- 0 = 
- 1 = 

### "UseDeathScreenStatistics"
Bool. If set to 1, enable the death statistics.
- 0 = 
- 1 = 

### "UseNewsFeedInGameMenu"
Bool. If set to 1, enable the expansion newsfeed in the pause menu.
- 0 = 
- 1 = 

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
        "EnableHUDGPS": 1,
        "NeedGPSItemForKeyBinding": 1,
        "NeedMapItemForKeyBinding": 1,
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