# This page is temporary, everything is subject to change

### WARNING! The lastest expansion update (1.02) for dayz 1.08 changed a lot of settings. It's highly recommended to regenerate your settings files !

* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/tree/development/ServerProfile/ExpansionMod/Settings) to see the server settings files
* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/commit/0a1f11b0e146bbf69a4c7af9aefbe034746159f1) to see the history of change for server settings

## Contents

- [AirdropSettings](#AirdropSettings)

- [BaseBuildingSettings](#BaseBuildingSettings)

- [BookSettings](#BookSettings)

- [GeneralSettings](#GeneralSettings)

- [MapSettings](#MapSettings)

- [MissionSettings](#MissionSettings)

- [NotificationSettings](#NotificationSettings)

- [PartySettings](#PartySettings)

- [SafeZoneSettings](#SafeZoneSettings)

- [SpawnSettings](#SpawnSettings)

- [TerritorySettings](#TerritorySettings)

- [VehicleSettings](#VehicleSettings)

====================================================================


# AirdropSettings

    {
        "Height": 0,
        "Speed": 0,
        "ItemCount": 50,
        "Containers": []
    }

### "Height"
DESCRIPTION

### "Speed"
DESCRIPTION

### "ItemCount"
The amount of items the airdrop will have in it.

### "Containers"
DESCRIPTION


# BaseBuildingSettings

    {
        "CanBuildAnywhere": 1,
        "AllowBuildingWithoutATerritory": 0,
        "AllowedItemsToPlaceEveryWhereButNotInEnemyTerritory": [
            "ExpansionSatchel",
            "Fireplace",
            "ExpansionFlagKitBase"
        ],
        "AllowedItemsToPlaceInEnemyTerritory": [
            "ExpansionSatchel"
        ],
        "CanCraftVanillaBasebuilding": 0,
        "CanCraftExpansionBasebuilding": 1,
        "CanCraftTerritoryFlag": 1,
        "DestroyFlagOnDismantle": 1,
        "CanDismantleFlag": 1,
        "DismantleOutsideTerritory": 0,
        "ExplosionTime": 30,
        "ExplosionDamageMultiplier": 50,
        "ProjectileDamageMultiplier": 1,
        "CanRaidSafes": 1,
        "SafeExplosionDamageMultiplier": 17,
        "SafeProjectileDamageMultiplier": 1,
        "CodeLockLength": 4,
        "DoDamageWhenEnterWrongCodeLock": 1,
        "DamageWhenEnterWrongCodeLock": 10
    }

### "CanBuildAnywhere"
DESCRIPTION

### "AllowBuildingWithoutATerritory"
Previously was TerritoryMode

### "AllowedItemsToPlaceEveryWhereButNotInEnemyTerritory"
WE FIXED THE TYPO IN THE NAME !

### "AllowedItemsToPlaceInEnemyTerritory"
WE FIXED THE TYPO IN THE NAME ! Yey !

### "CanCraftVanillaBasebuilding"
DESCRIPTION

### "CanCraftExpansionBasebuilding"
DESCRIPTION

### "CanCraftTerritoryFlag"
DESCRIPTION

### "DestroyFlagOnDismantle"
DESCRIPTION

### "CanDismantleFlag"
DESCRIPTION

### "DismantleOutsideTerritory"
DESCRIPTION

### "ExplosionTime"
DESCRIPTION

### "ExplosionDamageMultiplier"
DESCRIPTION

### "ProjectileDamageMultiplier"
DESCRIPTION

### "CanRaidSafes"
DESCRIPTION

### "SafeExplosionDamageMultiplier"
DESCRIPTION

### "SafeProjectileDamageMultiplier"
DESCRIPTION

### "CodeLockLength"
DESCRIPTION

### "DoDamageWhenEnterWrongCodeLock"
DESCRIPTION

### "DamageWhenEnterWrongCodeLock"
DESCRIPTION

# BookSettings

    {
        "EnableBook": 1,
        "EnableStatusTab": 1,
        "EnablePartyTab": 1,
        "EnableServerInfoTab": 1,
        "EnableServerRulesTab": 1,
        "EnableTerritoryTab": 1,
        "ShowServerSettings": 1,
        "ServerInfo": {
            "ServerButtons": [
                {
                    "IconPath": "set:expansion_iconset image:icon_group",
                    "URL": "https://exp.thurston.pw",
                    "Tooltip": "Feedback",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_discord",
                    "URL": "https://discord.io/expansion",
                    "Tooltip": "Discord",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_home",
                    "URL": "https://www.google.com",
                    "Tooltip": "Homepage",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_forums",
                    "URL": "https://www.google.com",
                    "Tooltip": "Forums",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_patreon",
                    "URL": "https://www.patreon.com/dayzexpansion",
                    "Tooltip": "Patreon",
                    "Color": -1
                }
            ],
            "ServerSections": [
                {
                    "HasHeading": 1,
                    "HeadText": "<p>PLACEHOLDER</p>",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "<p>PLACEHOLDER 2</p>",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "<p>PLACEHOLDER 3</p>",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "<p>PLACEHOLDER 4</p>",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "<p>PLACEHOLDER 5</p>",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>"
                }
            ],
            "ServerName": "SERVER NAME"
        },
        "ServerRules": {},
        "ServerLogoPath": "set:expansion_gui_logos image:expansion_logo_black"
    }

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

### "ShowServerSettings"
Bool. If enabled, the server settings will be visible in the server tab.

# GeneralSettings

    {
        "PlayerLocationNotifier": 1,
        "EnableHumanity": 0,
        "EnableGlobalChat": 1,
        "Mapping": {
            "UseCustomMappingModule": 0,
            "Mapping": [
                "BerezhkiCave",
                "Berezino",
                "Chernogorsk_Enhancement1",
                "Chernogorsk_Enhancement2",
                "Chernogorsk_Forest1",
                "Chernogorsk_Forest2",
                "Chernogorsk_Highschool",
                "DebugIsland",
                "Elektrozavodsk",
                "Evacuation",
                "Factory",
                "Gorka",
                "Kamenka",
                "Kamyshovo",
                "Krutoy_Cap",
                "Myshkino",
                "Nadezhdino",
                "Nizhnoye",
                "Novodmitrovsk",
                "Radom_Stuff",
                "Roads",
                "Sea_Platform",
                "Solnechniy",
                "Staroye",
                "StaryYarBkr",
                "Svetloyarsk",
                "Tisy",
                "BerezinoNoCollision",
                "Chernogorsk_Enhancement1NoCollision",
                "Chernogorsk_Enhancement2NoCollision",
                "Chernogorsk_Forest1NoCollision",
                "Chernogorsk_Forest2NoCollision",
                "Chernogorsk_Grass1NoCollision",
                "Chernogorsk_Grass2NoCollision",
                "Chernogorsk_HighschoolNoCollision",
                "DebugIslandNoCollision",
                "ElektrozavodskNoCollision",
                "EvacuationNoCollision",
                "GorkaNoCollision",
                "GrassNoCollision",
                "KamenkaNoCollision",
                "Kamyshovo_GrassNoCollision",
                "KamyshovoNoCollision",
                "Krutoy_CapNoCollision",
                "MyshkinoNoCollision",
                "NadezhdinoNoCollision",
                "Radom_StuffNoCollision",
                "RoadsNoCollision",
                "Solnechniy_GrassNoCollision",
                "StaroyeNoCollision",
                "StaryYarBkrNoCollision",
                "SvetloyarskNoCollision",
                "SvetRoadForestNoCollision",
                "TisyNoCollision"
            ],
            "ObjectsToDelete": [],
            "InteriorBuilding": 0,
            "Ivies": 0
        },
        "EnableLamps": 3,
        "EnableGenerators": 0,
        "EnableLighthouses": 1,
        "EnableHUDGPS": 1,
        "NeedGPSItemForKeyBinding": 1,
        "NeedMapItemForKeyBinding": 0,
        "EnableHUDNightvisionOverlay": 1,
        "DisableMagicCrosshair": 0,
        "EnablePlayerTags": 1,
        "PlayerTagViewRange": 5,
        "EnableHumanityOnPlayerTags": 0,
        "EnablePlayerList": 1,
        "EnableAutoRun": 1,
        "UnlimitedStamina": 0
    }

### "PlayerLocationNotifier"
Bool. When enabled, show to the player the name of the city he just got into and time of day

### "EnableHumanity" - CURRENTLY DOESNT WORK
Bool. This feature currentmy does nothing. 

### "UseCustomMappingModule"
Bool. When enabled, add custom mapping. Have a huge impact on server performance !

### "Mapping"
Array. List all the locations with custom mapping. 

### "ObjectsToDelete"
DESCRIPTION

### "InteriorBuilding"
Bool. When enabled, add more detailed interiors. Have a huge impact on server performance !

### "Ivies" - CURRENTLY DOESNT WORK
Bool. When enabled, allow ivies to be on some building. Only work for Chernarus !

### "LightingConfig"
Integer.

1. : Default - Default lighting of dayz we all know.
2. : Dark - Make the night very dark, the day is with default lighting.

### "EnableLamps"
Integer.

0. Disabled - The streets lights are off;
1. Generators - Currently unused. Would require you to fix a generator to make street lights work. - CURRENTLY DOESNT WORK
2. Always On - Street lights are emitting lights but some of them will stay off intentionnaly.
3. Always On (Everywhere) - Force every lights to be turned on;

### "EnableGenerators" - CURRENTLY DOESNT WORK
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

### "EnableHumanityOnPlayerTags" - CURRENTLY DOESNT WORK
Bool. If enabled, show the player tag Humanity when your cursor is on him.

### "EnablePlayerList"
Bool. If enabled, allow players to see the player list.

### "EnableAutoRun"
DESCRIPTION

### "UnlimitedStamina"
Bool. If enabled, make stamina unlimited.

### "VehicleSync"
Integer. Currently unused.

# MapSettings

    {
        "EnableMap": 1,
        "UseMapOnMapItem": 1,
        "CanCreateMarker": 1,
        "ShowPlayerPosition": 1,
        "CanCreatePartyMarkers": 1,
        "ShowMapStats": 1,
        "CanCreate3DMarker": 1,
        "ShowPartyMembersMapMarkers": 1,
        "ShowServerMarkers": 1,
        "CanOpenMapWithKeyBinding": 1,
        "ShowVehicleDebugMarkers": 0,
        "ServerMarkers": []
    }

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

### "ShowServerMarkers"
Bool. If enabled, show server map markers.

### "CanOpenMapWithKeyBinding"
Bool. If enabled, the player can open the map with a keybind instead of interacting with th physical map

### "ShowVehicleDebugMarkers"
DESCRIPTION

### "ServerMarkers"
Array. Allow server owners to display server markers on the map.
**TODO**

# MissionSettings

    {
        "Enabled": 1,
        "TimeBetweenMissions": 3600000,
        "MinMissions": 0,
        "MaxMissions": 1,
        "Missions": [
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\NameOfMyCustomAirdrop.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_NWAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_NWAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_NWAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_NWAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_NEAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_NEAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_NEAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_NEAF.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Berezino.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Berezino.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Berezino.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Berezino.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Balota.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Balota.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Balota.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Balota.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Zelenogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Zelenogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Zelenogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Zelenogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Myshkinko.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Myshkinko.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Myshkinko.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Myshkinko.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Novodmitrovsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Novodmitrovsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Novodmitrovsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Novodmitrovsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Chernogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Chernogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Chernogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Chernogorsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Elektrozavodsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Elektrozavodsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Elektrozavodsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Elektrozavodsk.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Skalisty-Island.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Skalisty-Island.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Skalisty-Island.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Skalisty-Island.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Sosnovka.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Sosnovka.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Sosnovka.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Sosnovka.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Novy-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Novy-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Novy-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Novy-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_General_Stary-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Medical_Stary-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Basebuilding_Stary-Sobor.json"
            },
            {
                "MissionType": "ExpansionMissionEventAirdrop",
                "MissionPath": "$profile:ExpansionMod\\Missions\\Airdrop_Military_Stary-Sobor.json"
            }
        ]
    }

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

# NotificationSettings

    {
        "EnableNotification": 1,
        "ShowPlayerJoinServer": 1,
        "JoinMessageType": 1,
        "ShowPlayerLeftServer": 1,
        "LeftMessageType": 1,
        "EnableKillFeed": 0,
        "KillFeedMessageType": 0,
        "ShowAirdropStarted": 1,
        "ShowAirdropClosingOn": 1,
        "ShowAirdropDropped": 1,
        "ShowPlayerAirdropStarted": 1,
        "ShowPlayerAirdropClosingOn": 1,
        "ShowPlayerAirdropDropped": 1,
        "ShowTerritoryNotifications": 1
    }

### "EnableNotification"
DESCRIPTION

### "ShowPlayerJoinServer"
DESCRIPTION

### "JoinMessageType"
DESCRIPTION

### "ShowPlayerLeftServer"
DESCRIPTION

### "LeftMessageType"
DESCRIPTION

### "EnableKillFeed"
DESCRIPTION

### "KillFeedMessageType"
DESCRIPTION

### "ShowAirdropStarted"
DESCRIPTION

### "ShowAirdropClosingOn"
DESCRIPTION

### "ShowAirdropDropped"
DESCRIPTION

### "ShowPlayerAirdropStarted"
DESCRIPTION

### "ShowPlayerAirdropClosingOn"
DESCRIPTION

### "ShowPlayerAirdropDropped"
DESCRIPTION

### "ShowTerritoryNotifications"
DESCRIPTION

# PartySettings

    {
        "EnableParties": 1,
        "MaxInParty": 10,
        "UseWholeMapForInviteList": 0,
        "ShowPartyMembers3DMarkers": 1,
        "DistanceForPartyMarkers": 2048,
        "EnableQuickMarker": 1,
        "ShowDistanceUnderQuickMarkers": 1
    }

### "EnableParties"
Bool. If enabled, allow players to create parties.

### "MaxInParty"
Integrer. Maximum of players allowed in a single party. If <= 0, unlimited party size.

### "UseWholeMapForInviteList"
Bool. If enabled, you can invite everyone from anywhere regardless of the distance.

### "ShowPartyMembers3DMarkers"
Bool. If enabled, show a 3d marker above the head of your teammates.

### "DistanceForPartyMarkers"
DESCRIPTION

### "EnableQuickMarker"
Bool. If enabled allow players to use QuickMarkers (act like a ping ingame).

### "ShowDistanceUnderQuickMarkers"
DESCRIPTION

# SafeZoneSettings

    {
        "Enabled": 0,
        "EnableVehicleinvincibleInsideSafeZone": 1,
        "FrameRateCheckSafeZoneInMs": 5000,
        "CircleZones": [
            {
                "Type": 1,
                "Center": [
                    11849.6,
                    0,
                    12471.6
                ],
                "Radius": 500
            }
        ],
        "PolygonZones": [
            {
                "Type": 2,
                "Positions": [
                    [
                        6345,
                        0,
                        2181
                    ],
                    [
                        6198,
                        0,
                        2433
                    ],
                    [
                        6565,
                        0,
                        2945
                    ],
                    [
                        7000,
                        0,
                        2521
                    ]
                ],
                "CenterPolygon": [
                    6561.09,
                    0,
                    2540.71
                ],
                "RadiusPolygon": 439.351
            }
        ]
    }

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

    {
        "StartingGear": {
            "UseStartingGear": 1,
            "UsingUpperGear": 1,
            "UsingPantsGear": 0,
            "UsingBackpackGear": 1,
            "SpawnBackpacks": [
                "TaloonBag_Blue",
                "TaloonBag_Green",
                "TaloonBag_Orange",
                "TaloonBag_Violet"
            ],
            "UpperGear": [
                "Rag",
                "Chemlight_White",
                "StoneKnife",
                "Apple"
            ],
            "PantsGear": [],
            "BackpackGear": [
                "SpaghettiCan",
                "BakedBeansCan"
            ]
        }
    }

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

    {
        "EnableTerritories": 1,
        "UseWholeMapForInviteList": 0,
        "TerritorySize": 150,
        "TerritoryPerimterSize": 150,
        "MaxMembersInTerritory": 10,
        "MaxTerritoryPerPlayer": -1
    }

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

# VehicleSettings

    {
        "VehicleSync": 0,
        "VehicleRequireKeyToStart": 1,
        "VehicleRequireAllDoors": 1,
        "VehicleLockedAllowInventoryAccess": 0,
        "VehicleLockedAllowInventoryAccessWithoutDoors": 1
    }

## "VehicleSync"
DESCRIPTION

## "VehicleRequireKeyToStart"
DESCRIPTION

## "VehicleRequireAllDoors"
DESCRIPTION

## "VehicleLockedAllowInventoryAccess"
DESCRIPTION

## "VehicleLockedAllowInventoryAccessWithoutDoors"
DESCRIPTION