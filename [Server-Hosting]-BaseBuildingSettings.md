Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)


***
### "CanBuildAnywhere"
Bool.
- 0 = Deploying an object and building vanilla fence/watchtower will follow the vanilla limitations.
- 1 = You can deploy anywhere and build anywhere without any restrictions from the vanilla limitations.

### "AllowBuildingWithoutATerritory"
Bool. 
- 0 = You are forced to build/deploy inside a territory. However You can add some objects to a whitelist if you still want some deployables usable outside the territory like a campfire or a beartrap.
- 1 = You are not restricted to only build/deploy inside a territory.

### "DeployableOutsideATerritory"
Array of string. Only used if TerritoryMode is set to 1. Put every classname of the item, you want to be able to be placed outside of the territory.

### "DeployableInsideAEnemyTerritory"
Array of string. Put every classname of the item, you want to be able to be placed in the territory where you are not a member of him.

### "CanCraftVanillaBasebuilding"
Bool.
- 0 = The player will not be able to craft the fence and watchtower kit.
- 1 = The player can craft the fence and watchtower kit.

### "CanCraftExpansionBasebuilding"
Bool.
- 0 = The player will not be able to craft all the expansion kits (wall, floor, ramp, stairs).
- 1 = The player can craft all the expansion kits (wall, floor, ramp, stairs).

### "DestroyFlagOnDismantle"
Bool.
- 0 = After dismantling the flag pole, you will get back your kit.
- 1 = You won't get your flag kit back after dismantling.

### "DismantleFlagRequireTools"
Bool.
- 0 = You can dismantle the flag pole with your hands.
- 1 = You need tools to dismantle the flag pole.

### "DismantleOutsideTerritory"
Bool.
- 0 = You cannot dismantle anything outside your own territory.
- 1 = You can dismantle everything unless if it's inside the territory of someone else.

### "DismantleAnywhere"
Bool.
- 0 = You need to be on the soft side of the object to have the dismantle action.
- 1 = The dismantle action will be available from anywhere. If you are in the territory of someone else, you won't be able to dismantle.

### "CodeLockLength"
Integer. The length of passwords you can put into your code locks.

### "DoDamageWhenEnterWrongCodeLock"
Bool.
- 0 = If the user give the wrong password he won't get hurt.
- 1 = If the password is wrong, he will get hurt by the amount defined in "DamageWhenEnterWrongCodeLock".

### "DamageWhenEnterWrongCodeLock"
Float. The number of damage the player will take when he types a wrong code lock. 0 won't do anything damage and 100 will kill the player.

### "CanCraftTerritoryFlagKit"
Bool.
- 0 = The player can't craft the territory flag.
- 1 = The player can craft the territory flag (3 sticks + 1 rope).

### "SimpleTerritory"
Bool.
- 0 = The player will have to build the flag pole like in vanilla.
- 1 = The flag pole will be built automaticly after being deployed.

### "AutomaticFlagOnCreation"
Bool.
- 0 = The player will need to add by himself the flag.
- 1 = The flag will be automaticly added to the flag pole.

### "EnableFlagMenu"
Bool.
- 0 = The player will not be able to create a territory.
- 1 = The player will be able to create a territory to protect his base.

### "GetTerritoryFlagKitAfterBuild"
Bool.
- 0 = The player will not get his kit after building his territory flag.
- 1 = The player will get his kit back after building the first stage of the territory flag.

***

    {
        "CanBuildAnywhere": 1,
        "AllowBuildingWithoutATerritory": 1,
        "DeployableOutsideATerritory": [
            "ExpansionSatchel",
            "Fireplace",
            "TerritoryFlagKit"
        ],
        "DeployableInsideAEnemyTerritory": [
            "ExpansionSatchel",
            "LandMineTrap",
            "BearTrap"
        ],
        "CanCraftVanillaBasebuilding": 0,
        "CanCraftExpansionBasebuilding": 1,
        "DestroyFlagOnDismantle": 1,
        "DismantleFlagRequireTools": 1,
        "DismantleOutsideTerritory": 0,
        "DismantleAnywhere": 0,
        "CodeLockLength": 4,
        "DoDamageWhenEnterWrongCodeLock": 1,
        "DamageWhenEnterWrongCodeLock": 10,
        "CanCraftTerritoryFlagKit": 1,
        "SimpleTerritory": 1,
        "AutomaticFlagOnCreation": 1,
        "EnableFlagMenu": 1,
        "GetTerritoryFlagKitAfterBuild": 0
    }