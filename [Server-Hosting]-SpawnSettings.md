Last updated the 20th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***
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
			"UseCustomClothing": 0,
			"Headgear": [],
			"Glasses": [],
			"Masks": [],
			"Tops": [
				"TShirt_Green"
			],
			"Vests": [],
			"Gloves": [],
			"Pants": [
				"TrackSuitPants_Black",
				"TrackSuitPants_Red",
				"TrackSuitPants_Green"
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
			"UseStartingGear": 0,
			"UsingUpperGear": 0,
			"UsingPantsGear": 0,
			"UsingBackpackGear": 0,
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