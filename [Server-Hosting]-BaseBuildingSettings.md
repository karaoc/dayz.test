Last updated the 24th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)


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
Array of string. Only used if AllowBuildingWithoutATerritory is set to 0. This list of classnames are the items you will be able to deploy outside the territories.

Example : 

    "DeployableOutsideATerritory": [
        "classname01_withaCommaAtTheEnd",
        "classname02_withaCommaAtTheEnd",
        "classname03_withoutCommaAtTheEndBecauseItsTheLastOne"
    ],

### "DeployableInsideAEnemyTerritory"
Array of string. This list is used for raiding purposes. All the classnames listed here will be deployable inside the territory of your ennemies. It's recommended to only allow raiding devices or traps.

Example : 

    "DeployableInsideAEnemyTerritory": [
        "classname01_withaCommaAtTheEnd",
        "classname02_withaCommaAtTheEnd",
        "classname03_withoutCommaAtTheEndBecauseItsTheLastOne"
    ],

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
Integrer.
- -1 = Only territory members can dismantle the flag pole.
- 0 = You can dismantle the flag pole with your hands.
- 1 = You need tools to dismantle the flag pole.

### "DismantleOutsideTerritory"
Bool.
- 0 = You cannot dismantle anything outside your own territory.
- 1 = You can dismantle everything unless if it's inside the territory of someone else.

### "DismantleInsideTerritory"
Bool.
- 0 = You cannot dismantle anything inside the territories you don't own.
- 1 = You can dismantle inside the territory of everyone.

### "DismantleAnywhere"
Bool.
- 0 = You need to be on the soft side of the object to have the dismantle action.
- 1 = The dismantle action will be available from anywhere. If you are in the territory of someone else, you won't be able to dismantle.

### "CodelockActionsAnywhere"
Bool.
- 0 = You need to look at the codelock to have the interactions with the codelock. (like in vanilla)
- 1 = You need to look at the wall, door, gate or the codelock to get the interactions with the codelock. (like codelock mod)

### "CodeLockLength"
Integer. The length of passwords you can put into your code locks. If you want to only allow 6 digits password in the codelocks set it to 6 for example.

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
Integrer.
- 0 = The player will not be able to create a territory.
- 1 = The player will be able to create a territory to protect his base.
- 2 = The player will be able to create a territory to protect his base but he won't be able to customize his flag from the flag menu.

### "GetTerritoryFlagKitAfterBuild"
Bool.
- 0 = The player will not get his kit after building his territory flag.
- 1 = The player will get his kit back after building the first stage of the territory flag.

Since this is currently the last setting you don't need the comma at the end !

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/BaseBuildingSettings.json