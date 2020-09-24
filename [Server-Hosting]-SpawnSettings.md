Last updated the 20th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

This file have been updated with the lastest update. I will do a complete documentation update later. But I still want to give you something to help you a bit. Here are the dev comments we have to explain this settings on our side : 

    StartingClothing:
    "UseCustomClothing" renamed to "EnableCustomClothing"
    New setting "SetRandomHeath" // When enabled it will add random damage to the clothing items with that a player spawn.

    StartingGear:
    "UseStartingGear" renamed to "EnableStartingGear"
    "UseingUpperGear" renamed to "UseUpperGear"
    "UseingPantsGear" renamed to "UsePantsGear"
    "UseingBackpackGear" renamed to "UseBackpackGear"
    New setting bool "UsePrimaryWeapon" // When enabled player will spawn with the primary weapon configured in the PrimaryWeapon string.
    New setting bool "UseSecondaryWeapon" // When enabled player will spawn with the primary weapon configured in the SecondaryWeapon string.
    New setting bool "UseVestGear" // When enabled player will spawn with the gear configured in the VestGear string array.
    New setting string array "VestGear" // String array for items that get spawned into the players vest.
    New setting "PrimaryWeapon" // String for the item that get spawned into the players primary weapon slot.
    New setting "PrimaryWeaponAttachments" // String array for attachments that get attached to the players primary weapon.
    New setting "SecondaryWeapon" // String for the item that get spawned into the players shoulder slot.
    New setting "SecondaryWeaponAttachments" // String array for attachments that get attached to the players secondary weapon.
    New setting "ApplyEnergySources" // If enabled then all items that need a V9 batterie in players inventory a batterie attached.
    New setting "SetRandomHeath" // When enabled it will add random damage to the gear items with that a player spawn.

### "UseCustomClothing"
Bool.
- 0 = The player will spawn with the vanilla default clothing items attached to his character
- 1 = The player will spawn with the configured clothing items in this file

### "Headgear"
Array.
- List of classnames used for the custom clothing.

Need to be headgear attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Glasses"
Array.
- List of classnames used for the custom clothing.

Need to be eyewear attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Masks"
Array.
- List of classnames used for the custom clothing.

Need to be masks attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Tops"
Array.
- List of classnames used for the custom clothing.

Need to be tops/shirts/jackets attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Vests"
Array.
- List of classnames used for the custom clothing.

Need to be vests attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Gloves"
Array.
- List of classnames used for the custom clothing.

Need to be gloves attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Pants"
Array.
- List of classnames used for the custom clothing.

Need to be pants/shorts attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Belts"
Array.
- List of classnames used for the custom clothing.

Need to be belts attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Shoes"
Array.
- List of classnames used for the custom clothing.

Need to be shoes attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Armbands"
Array.
- List of classnames used for the custom clothing.

Need to be armabands attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "Backpacks"
Array.
- List of classnames used for the custom clothing.

Need to be backpacks attachments/items!
If the array only contains one item classname it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise the item will be selected randomly.

### "UseStartingGear"
Bool.
- 0 = The player will spawn with the vanilla default gear
- 1 = The player will spawn with the configured gear in this file

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
Array. 
- List of classnames used for the items spawning inside the backpack

### "UpperGear"
Array. 
- List of classnames used for the upper gear

### "PantsGear"
Array. 
- List of classnames used for the pants gear

### "BackpackGear"
Array.
- List of classnames used for the backpack gear

# Raw file

    {
        "StartingClothing": {
            "EnableCustomClothing": 1,
            "SetRandomHeath": 1,
            "Headgear": [],
            "Glasses": [],
            "Masks": [],
            "Tops": [
                "TShirt_Green",
                "TShirt_Blue",
                "TShirt_Black",
                "TShirt_Beige",
                "TShirt_Red",
                "TShirt_OrangeWhiteStripes",
                "TShirt_White",
                "TShirt_Red",
                "TShirt_Grey",
                "TShirt_RedBlackStripes"
            ],
            "Vests": [],
            "Gloves": [],
            "Pants": [
                "CanvasPants_Beige",
                "CanvasPants_Blue",
                "CanvasPants_Grey",
                "CanvasPants_Red",
                "CanvasPants_Violet",
                "CanvasPantsMidi_Beige",
                "CanvasPantsMidi_Blue",
                "CanvasPantsMidi_Grey",
                "CanvasPantsMidi_Red",
                "CanvasPantsMidi_Violet"
            ],
            "Belts": [],
            "Shoes": [
                "AthleticShoes_Blue",
                "AthleticShoes_Grey",
                "AthleticShoes_Brown",
                "AthleticShoes_Green",
                "AthleticShoes_Black"
            ],
            "Armbands": [],
            "Backpacks": [
                "TaloonBag_Blue",
                "TaloonBag_Green",
                "TaloonBag_Orange",
                "TaloonBag_Violet"
            ]
        },
        "StartingGear": {
            "EnableStartingGear": 1,
            "UseUpperGear": 1,
            "UsePantsGear": 0,
            "UseBackpackGear": 1,
            "UseVestGear": 0,
            "UsePrimaryWeapon": 0,
            "UseSecondaryWeapon": 0,
            "UpperGear": [
                "Rag",
                "StoneKnife",
                "Apple"
            ],
            "PantsGear": [],
            "BackpackGear": [
                "SpaghettiCan",
                "BakedBeansCan",
                "Chemlight_White"
            ],
            "VestGear": [],
            "PrimaryWeapon": "",
            "PrimaryWeaponAttachments": [],
            "SecondaryWeapon": "",
            "SecondaryWeaponAttachments": [],
            "ApplyEnergySources": 1,
            "SetRandomHeath": 1
        }
    }