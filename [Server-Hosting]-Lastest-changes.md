### Please think to update your server settings after each updates !

# Update 1.05.xxxxxx

You can download the server setting files from this link : 

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings

You can see all the changes in the server settings with this link: 

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/commit/9689540d1884918af48709a9b4ef47de8707d1da

## Mission files

The lastest mission files are now up to date with dayz 1.10. We have also added back a DayZ pistol, the LongHorn !

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions/releases/

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions

## SpawnSettings.json

| Added| Why |
|---|---|
| EnableSpawnSelection | To allow servers to disable Expansion Spawn Selection if they don't want to use it |
| SpawnSelectionScreenMenuID | This setting should allow server hosters to create their own custom menu for the spawn selection |
| SpawnOnTerritory | To allow servers to let their players respawn inside their bases if they want to |
| SpawnLocations | Will allow servers to have custom spawn locations and keep them a bit randomized if they want to |

    "SpawnLocations": [
        {
            "Name": "My Location Name",
            "Positions": [
                [
                    100,    | Potential spawn 1
                    2,      | If only one Position is set, the player will always spawn at this position
                    50      | Also, the first spawn position will be used to create the 2d marker on the map
                ],
                [
                    250,    |
                    2.75,   | Potential spawn 2
                    100     |
                ]
            ]
        },
        {
            "Name": "Berezino",
            "Positions": [
                [
                    12915.7001953125,
                    3.4000000953674318,
                    9278.2001953125
                ],
                [
                    13057.2001953125,
                    2.299999952316284,
                    9584.48046875
                ],
                [
                    13052.900390625,
                    6.099999904632568,
                    9894.7001953125
                ],
                [
                    13207.2001953125,
                    2.299999952316284,
                    10193.7001953125
                ]
            ]
        }
    ]

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-SpawnSettings)

## DebugSettings.json

| Added| Why |
|---|---|
| DebugVehicleSync | This setting is for debug purpose only ! |
| DebugVehicleTransformSet | This setting is for debug purpose only ! |
| DebugVehiclePlayerNetworkBubbleMode| This setting is for debug purpose only ! |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-DebugSettings)

## VehicleSettings.json

| Updated| Added| Why |
|---|---|---|
|| EnableHelicopterExplosions | This should help servers with the Helicopters Explosions issue until further investigation is done |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-VehicleSettings)

## MapSettings.json

| Updated | Added | Why |
|---|---|---|
|| NeedPenItemForCreateMarker | Requested by Roleplay servers. If you don't have a pen on you, you won't be able to create markers |
| ShowPlayerPosition || Now this setting can also be set to 2. This mode will require the player to have a compass on him to see his player position |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-MapSettings)

## GeneralSettings.json

| Added| Why |
|---|---|
| Interiors | You can now keep custom interiors enabled but only for the buildings you want to |

For example, if you only want custom interiors in industrial and rural buildings you should have a similar result : 

    "Interiors": [
        "Land_Barn_Brick2",
        "Land_Barn_Metal_Big",
        "Land_Barn_Wood2",
        "Land_BarnMetal_Big_Grey",
        "Land_Garage_Big",
        "Land_Garage_Row_Big",
        "Land_Shed_Closed",
        "Land_Power_Station",
        "Land_Rail_Station_Big"
    ],

Here is a list of all the buildings classnames configured to spawn with a custom interior [click on this link](https://pastebin.com/DbFcM4ZT).

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-GeneralSettings)

## NotificationSettings.json

| Added| Why |
|---|---|
| ShowAirdropEnded | This setting was missing. Now you can hide the notification "The Airdrop at ... was destroyed by infected." |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-NotificationSettings)

## BaseBuildingSettings.json

| Added| Why |
|---|---|
| DismantleInsideTerritory | Allow raiders to have the dismantle action inside a territory they don't own |
| CodelockActionsAnywhere | To allow players to interact with the codelock on expansion walls even if they are not looking at the codelock himself |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings)

## BookSettings.json

| Before | After | Added | Why |
|---|---|---|---|
||| ItemRequired | Requested by some Roleplay servers. If this setting have a classname in "", the player will need to find this item to open his book|
||| ItemRequiredLocation | This setting allow server hosters to choose if they want to require the item to be in the hands of the player or not. 0 = required to be in the inventory and 1 = required to be in the hands of the player |
| RuleCategorys | RuleCategories || Typo in the name, it have been changed in this update since this is a major update. Go inside your booksettings.json and rename setting. |

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BookSettings)