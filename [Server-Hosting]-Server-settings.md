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

- [RaidSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-RaidSettings)

- [SafeZoneSettings](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-SafeZoneSettings)

- [SpawnSettings](#SpawnSettings)

- [TerritorySettings](#TerritorySettings)

- [VehicleSettings](#VehicleSettings)


***

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