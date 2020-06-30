![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

### Please think to update your server settings after each updates !

* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/tree/master/ServerProfile/ExpansionMod/Settings) to see the server settings files
* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/commit/befd7e7cfee6a85f4cc1b26326e5d6c6a4b11ed7) to see the lastest changes for server settings
* [Click me](https://github.com/salutesh/DayZ-Expansion-Scripts/commits/master/ServerProfile/ExpansionMod/Settings) to see the history of changes for server settings

## Contents

- [AirdropSettings](#AirdropSettings)

- [BaseBuildingSettings](#BaseBuildingSettings)

- [BookSettings](#BookSettings)

- [GeneralSettings](#GeneralSettings)

- [MapSettings](#MapSettings)

- [MissionSettings](#MissionSettings)

- [NotificationSettings](#NotificationSettings)

- [PartySettings](#PartySettings)

- [RaidSettings](#RaidSettings)

- [SafeZoneSettings](#SafeZoneSettings)

- [SpawnSettings](#SpawnSettings)

- [TerritorySettings](#TerritorySettings)

- [VehicleSettings](#VehicleSettings)


***


# AirdropSettings

    {
        "Height": 0,
        "Speed": 0,
        "ItemCount": 50,
        "Containers": []
    }

### "Height"
The altitude the plane will fly at.

### "Speed"
Float. The speed of the plane.

### "ItemCount"
The amount of items the airdrop will have in it.

### "Containers"
What loot could spawn inside the airdrop. You have to give the Name of the Classname, his chance of spawning (1.00 = 100%) and his attachements if you want it to spawn with items attached to it. Please make sure the last } of the loot list doesn't have the , in }, like in the example !


# BaseBuildingSettings

    {
        "CanBuildAnywhere": 1,
        "AllowBuildingWithoutATerritory": 0,
        "DeployableOutsideATerritory": [
            "ExpansionSatchel",
            "Fireplace",
            "ExpansionFlagKitBase"
        ],
        "DeployableInsideAEnemyTerritory": [
            "ExpansionSatchel"
        ],
        "CanCraftVanillaBasebuilding": 0,
        "CanCraftExpansionBasebuilding": 1,
        "CanCraftTerritoryFlag": 1,
        "DestroyFlagOnDismantle": 1,
        "CanDismantleFlag": 1,
        "DismantleOutsideTerritory": 0,
        "CodeLockLength": 4,
        "DoDamageWhenEnterWrongCodeLock": 1,
        "DamageWhenEnterWrongCodeLock": 10
    }

### "CanBuildAnywhere"
Bool. If set to 1, allow to build any where.

### "AllowBuildingWithoutATerritory"
Bool. Previously known as TerritoryMode, if set to one allow to build without the need of a territory

### "DeployableOutsideATerritory"
Array of string. Only used if TerritoryMode is set to 1. Put every classname of the item, you want to be able to be placed outside of the territory.

### "DeployableInsideAEnemyTerritory"
Array of string. Put every classname of the item, you want to be able to be placed in the territory where you are not a member of him.

### "AllowedItemsToPlaceEveryWhereButNotInEnemyTerritory"
Array of string. Only used if AllowBuildingWithoutATerritory is set to 1. Put every classname of the item, you want to be able to be placed outside of the territory.

### "AllowedItemsToPlaceInEnemyTerritory"
Array of string. Put every classname of the item, you want to be able to be placed in the territory where you are not a member of him.

### "CanCraftVanillaBasebuilding"
Bool. If set to 0, you can not craft vanilla basebuilding objects (FenceKit and WatchTowerKit). If 1, you can.

### "CanCraftExpansionBasebuilding"
Bool. If set to 0, you can not craft DayZ Expansion Basebuilding objects.

### "CanCraftTerritoryFlag"
Bool. If set to 0, remove the craft recipe for expansion flags which are used for the territory system.

### "DestroyFlagOnDismantle"
Bool. If set to 1, destroy the flag after dismantling it.

### "CanDismantleFlag"
Bool. If set to 1, allow the player to dismantle flags.

### "DismantleOutsideTerritory"
Bool. If set to 1, allow to dismantle outside territories.

### "CodeLockLength"
Integer. The length of passwords you can put into your code locks.

### "DoDamageWhenEnterWrongCodeLock"
Bool. If set to 0, the player will not take damage if he enters a wrong code lock. If set to 1, he will take damage.

### "DamageWhenEnterWrongCodeLock"
Float. The number of damage the player will take when he types a wrong code lock.

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
        "ServerRules": {
            "RuleSections": [
                {
                    "Lable": "General Rules",
                    "RulesPages": [
                        {
                            "HeadText": "Rule 1",
                            "BodyText": "This is a simple test text."
                        },
                        {
                            "HeadText": "Rule 2",
                            "BodyText": "This is a simple test text."
                        }
                    ],
                    "PageSections": [
                        {
                            "Left": 0,
                            "Right": 0
                        },
                        {
                            "Left": 0,
                            "Right": 1
                        }
                    ]
                }
            ]
        },
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

### "ServerInfo"
Array. Allow to write multiple paragraph to share informations about the server. A guide is [available here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-the-Server-Book-Tab)

### "ServerRules"
Array. This where you will organize and list your rules for your server. **This feature is currently NOT finished and NOT ready**.

### "ServerLogoPath"
String. Parameter for the logo of the server. Need to be in EDDS format and inside a mod. a url won't work.


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
        "UnlimitedStamina": 0,
        "DisableDamagedHeliSpin": 1
    }

### "PlayerLocationNotifier"
Bool. When enabled, show to the player the name of the city he just got into and time of day

### "EnableHumanity" - CURRENTLY DOESNT WORK
Bool. This feature currentmy does nothing. 

### "UseCustomMappingModule"
Bool. if set to 1, add custom mapping. Have a huge impact on server performance !

### "Mapping"
Array. List all the locations with custom mapping. 

### "ObjectsToDelete"
Array. You can indicate the position and the name of a specific mapped object to be removed. This action can be done to multiple objects.

### "InteriorBuilding"
Bool. if set to 1, add more detailed interiors. Have a huge impact on server performance !

### "Ivies" - CURRENTLY DOESNT WORK
Bool. if set to 1, allow ivies to be on some building. Only work for Chernarus !

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
Bool. If set to 1, turns on the light of every lighthouses of the map.

### "EnableAutoRun"
Bool. If set to 1, allow the player to autojog.

### "NeedGPSItemForKeyBinding"
Bool. If set to 1, require the player to have the GPS item in his inventory to open the GPS

### "NeedMapItemForKeyBinding"
Bool. If set to 1, require the player to have the map item in his inventory to open the map

### "EnableHUDNightvisionOverlay"
Bool. If set to 1, add a immersive NVG overlay

### "EnablePlayerTags"
Bool. If set to 1, show the player tag when your cursor is on him.

### "PlayerTagViewRange"
Integer. Distance requiried to see the tag. The value is in meter, in other words 5 is 5 meters.

### "EnableHumanityOnPlayerTags" - CURRENTLY DOESNT WORK
Bool. If set to 1, show the player tag Humanity when your cursor is on him.

### "EnablePlayerList"
Bool. If set to 1, allow players to see the player list.

### "EnableAutoRun"
Bool. If set to 1, allow the player to use the autorun feature.

### "UnlimitedStamina"
Bool. If enabled, make stamina unlimited.

### "DisableDamagedHeliSpin"
Bool. If set to 1, will disable helicopters from taking any damage.

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
Array. Allow server owners to display server markers on the map. See [this tutorial](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-server-markers) for more explaination.

# MissionSettings

    {
        "Enabled": 1,
        "TimeBetweenMissions": 3600000,
        "MinMissions": 0,
        "MaxMissions": 1,
        "Missions": [
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

### "Missions"
Array. List the missions configured on the server. Currently only used for [airdrops](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-custom-airdrops).

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
Bool. If set to 1, enable to notifications for everyone.

### "ShowPlayerJoinServer"
Bool. If set to 1, notify the player who joined the server.

### "JoinMessageType"
Integer. with 2 modes :

0. Will display the player joined message in the globalchat
1. Will display the player joined message in a notification

### "ShowPlayerLeftServer"
Bool. If set to 1, notify the player who left the server.

### "LeftMessageType"
Integer. with 2 modes :

0. Will display the player left message in the globalchat
1. Will display the player left message in a notification

### "EnableKillFeed" - CURRENTLY DOESNT WORK
Bool. If set to 1, notify the player of whom got killed and how.

### "KillFeedMessageType"
Integer. with 2 modes :

0. Will display the player left message in the globalchat
1. Will display the player left message in a notification

### "ShowAirdropStarted"
Bool. If set to 1, will notify the player a airdrop just started.

### "ShowAirdropClosingOn"
Bool. If set to 1, will notify the player a airdrop is getting closer.

### "ShowAirdropDropped"
Bool. If set to 1, will notify the player a airdrop dropped the package.

### "ShowPlayerAirdropStarted"
Bool. If set to 1, will notify the player a airdrop called by a player just started.

### "ShowPlayerAirdropClosingOn"
Bool. If set to 1, will notify the player a airdrop called by a player is getting closer.

### "ShowPlayerAirdropDropped"
Bool. If set to 1, will notify the player a airdrop called by a player dropped the package.

### "ShowTerritoryNotifications"
Bool. If set to 1, will notify the player he entered/left a territory.

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
Integrer. Distance in meters before the 3d marker fade out. Could not go over bubble network distance ~1000 m per default in DayZ

### "EnableQuickMarker"
Bool. If set to 1, allow players to use QuickMarkers (act like a ping ingame).

### "ShowDistanceUnderQuickMarkers"
Bool. If set to 1, show the distance between you and your quickmarker.

# RaidSettings

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
        "SafeProjectileDamageMultiplier": 1,
        "AllowMeleeRaidingOnVanilla": 0,
        "AllowMeleeRaidingOnExpansion": 0
    } 


### "ExplosionTime"
Integer. Time in seconds it takes for a ExpansionExplosiveBase to countdown and detonate.

### "ExplosiveDamageWhitelist"
Array of string. Put every classname of the explosive items you want to be able to be used for raiding.

### "EnableExplosiveWhitelist"
Bool. If set to 1, only the items listed above will be able to raid basebuilding elements.

### "ExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the wall, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. Less than 1 values work here as well, so 0x will disable damage to base parts, and .5x will halve them. Note, walls currently have an HP of 30,000.

### "ProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the wall, so 130.** Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, walls currently have an HP of 30,000.

### "CanRaidSafes"
Bool. If set to 1, allow to players to raid expansion safes.

### "SafeExplosionDamageMultiplier"
Float. It is a damage multiplier for all explosion type damages to Expansion base parts. For example with the default value of 50, a grenade that does 50 damage will do 50 * 50 damage to the safe, so 2500. For reference, vanilla grenades do 50 damage, Expansion rockets do 300, and C4 does 600. Less than 1 values work here as well, so 0x will disable damage to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

### "SafeProjectileDamageMultiplier"
Float. It is a damage multiplier for all bullet type damages to Expansion base parts. For example with the default value of 2, a bullet that does 65 damage will do 65 * 2 damage to the safe, so 130.** Less than 1 values work here as well, so 0x will disable damage** to base parts, and .5x will halve them. Note, safes currently have 20,000 15,000 and 10,000 HP.

### "AllowMeleeRaidingOnVanilla" -- CURRENTLY NOT WORKING
Bool. If set to 1, allow melee items to raid vanilla basebuilding.

### "AllowMeleeRaidingOnExpansion" -- CURRENTLY NOT WORKING
Bool. If set to 1, allow melee items to raid Expansion basebuilding.

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
        "MaxTerritoryPerPlayer": 1
    }

### "EnableTerritories"
Bool. If enabled, use the expansion territory system

### "UseWholeMapForInviteList"
Bool. If enabled, will make the whole map available in invite list, instead only nearby players.

### "TerritorySize"
Float. the radius of territory in meters.

### "TerritoryPerimterSize"
Float. A perimeter surrounding a territory to prevent other territories to be built in. It will prevent territories to overlap if the value set is the same as TerritorySize or higher.
![perimeter sheet](https://i.imgur.com/gJX5Ula.png)

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

### "VehicleSync" - CURRENTLY DOESNT WORK
Integrer. with x modes :

0. Will change the Vehicle sync to...
1. Will change the Vehicle sync to...

### "VehicleRequireKeyToStart"
Bool. If set to 1, you will need a car key paired to the vehicle to start the engine.

### "VehicleRequireAllDoors"
Bool. If set to 1, you will need all the doors of the car to lock your vehicle.

### "VehicleLockedAllowInventoryAccess"
Bool. If set to 1, allow players to access the inventory of the vehicle even if this vehicle is locked.

### "VehicleLockedAllowInventoryAccessWithoutDoors"
Bool. If set to 1, allow players to access inventory of the vehicle only if this vehicle is missing one or multiple doors.