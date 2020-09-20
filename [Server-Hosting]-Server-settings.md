### Please think to update your server settings after each updates !

## Contents

- [AirdropSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-AirdropSettings)

- [BaseBuildingSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings)

- [BookSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BookSettings)

- [DebugSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-DebugSettings)

- [GeneralSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-GeneralSettings)

- [MapSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-MapSettings)

- [MissionSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-MissionSettings)

- [NotificationSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-NotificationSettings)

- [PartySettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-PartySettings)

- [RaidSettings](#RaidSettings)

- [SafeZoneSettings](#SafeZoneSettings)

- [SpawnSettings](#SpawnSettings)

- [TerritorySettings](#TerritorySettings)

- [VehicleSettings](#VehicleSettings)


***

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
        "SafeProjectileDamageMultiplier": 1
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
- Type: Tell which type of safezone it is (circular or polygon) by indicating 1 or 2. For a CircleZones it's 1
- Center: where the zone should be on the map
- Radius: Size of the zone

### "PolygonZones"
Array.
- Type: Tell which type of safezone it is (circular or polygon) by indicating 1 or 2. For a PolygonZones it's 2
- Positions: A array of positions to draw this polygon.
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
        "TerritoryPerimeterSize": 150,
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
        "VehicleSync": 1,
        "VehicleRequireKeyToStart": 1,
        "VehicleRequireAllDoors": 1,
        "VehicleLockedAllowInventoryAccess": 0,
        "VehicleLockedAllowInventoryAccessWithoutDoors": 1,
        "EnableWindAerodynamics": 1,
        "EnableTailRotorDamage": 1,
        "PlayerAttachment": 1,
        "Towing": 1
    }

### "VehicleSync" - CURRENTLY DOESNT WORK
Integrer. with x modes :

0. Will change the Vehicle sync to...
1. Will change the Vehicle sync to...
2. Will change the Vehicle sync to...

### "VehicleRequireKeyToStart"
Bool. If set to 1, you will need a car key paired to the vehicle to start the engine.

### "VehicleRequireAllDoors"
Bool. If set to 1, you will need all the doors of the car to lock your vehicle.

### "VehicleLockedAllowInventoryAccess"
Bool. If set to 1, allow players to access the inventory of the vehicle even if this vehicle is locked.

### "VehicleLockedAllowInventoryAccessWithoutDoors"
Bool. If set to 1, allow players to access inventory of the vehicle only if this vehicle is missing one or multiple doors.

### "EnableWindAerodynamics"
Bool. If set to 1, enable wind simulation for helicopters.

### "EnableTailRotorDamage"
Bool. If set to 1, rotors of helicopters can be damaged and will spin if destroy making the helicopters almost unusable.

### "PlayerAttachment"
Bool. If set to 1, allow players to stay on moving objects like cars, helicopters, planes or boats.

### "Towing"
Bool. If set to 1, allow cars to tow other cars. Helicopters can tow any types vehicles.