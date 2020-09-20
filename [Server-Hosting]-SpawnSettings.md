Last updated the 20th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "UseStartingGear"
Bool.
- 0 = The player will spawn with the vanilla default gear
- 1 = The player will spawn with the configured gear in this file.

### "UsingUpperGear"
Bool.
- 0 = The "UpperGear" will not be used. Nothing from this list will spawn
- 1 = The items from "UpperGear" will be added into the inventory of the player in his Upper inventory (shirt inventory)

### "UsingPantsGear"
Bool.
- 0 = The "PantsGear" will not be used. Nothing from this list will spawn
- 1 = The items from "PantsGear" will be added into the inventory of the player in his Pant inventory

### "UsingBackpackGear"
Bool.
- 0 = The "BackpackGear" will not be used. Nothing from this list will spawn
- 1 = The items from "BackpackGear" will be added into the inventory of the player in his backpack inventory

### "SpawnBackpacks"
Array. list of classnames used for the items spawning inside the backpack

### "UpperGear"
Array. list of classnames used for the upper gear

### "PantsGear"
Array. list of classnames used for the pants gear

### "BackpackGear"
Array. list of classnames used for the backpack gear

# Raw file

    {
        "StartingGear": {
            "UseStartingGear": 1,
            "UsingUpperGear": 1,
            "UsingPantsGear": 0,
            "UsingBackpackGear": 1,
            "UpperGear": [],
            "PantsGear": [],
            "BackpackGear": []
        },
        "UseCustomClothing": 1,
        "StartingClothing": {
            "Headgear": [],
            "Glasses": [],
            "Masks": [],
            "Tops": [],
            "Vests": [],
            "Gloves": [],
            "Pants": [],
            "Belts": [],
            "Shoes": [ ],
            "Armbands": [],
            "Backpacks": []
        }
    }