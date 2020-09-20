Last updated the 20th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***
### "EnableTerritories"
Bool.
- 0 = The Territory flag will only have the vanilla functionnality.
- 1 = Will enable Expansion Territory system.

### "UseWholeMapForInviteList"
Bool.
- 0 =  The player can only invite players in his territory if they are near him.
- 1 = The player can invite anyone in his territory, even if they are on the other side of the map.

### "TerritorySize"
Float. the radius of territory in meters.

### "TerritoryPerimterSize"
Float. A perimeter surrounding a territory to prevent other territories to be built in. It will prevent territories to overlap if the value set is the same as TerritorySize or higher.
![perimeter sheet](https://i.imgur.com/gJX5Ula.png)

### "MaxMembersInTerritory"
Integer. The max amount of members allowed per territories. If <= 0, unlimited territory size.

### "MaxTerritoryPerPlayer"
Integer. The max amount of territories allowed per player. If <= 0, unlimited territory allowed.

# Raw file

    {
        "EnableTerritories": 1,
        "UseWholeMapForInviteList": 0,
        "TerritorySize": 150,
        "TerritoryPerimeterSize": 150,
        "MaxMembersInTerritory": 10,
        "MaxTerritoryPerPlayer": 1
    }