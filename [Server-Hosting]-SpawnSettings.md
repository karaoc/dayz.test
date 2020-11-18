Last updated the 19th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

# Starting Clothing:
### "EnableCustomClothing"
Bool.
- 0 = The player will spawn with the vanilla default clothing items attached to his character
- 1 = The player will spawn with the configured clothing items in this file

### "SetRandomHealth"
Bool.
- 0 = All the clothing items with that the player spawns are in a pristine condition
- 1 = All the clothing items with that the player spawns are in a random condition

### "Headgear"
Array.
- List of class names used for the custom clothing.

Need to be headgear attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Glasses"
Array.
- List of class names used for the custom clothing.

Need to be eyewear attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Masks"
Array.
- List of class names used for the custom clothing.

Need to masks attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Tops"
Array.
- List of class names used for custom clothing.

Need to be top/shirts/jackets attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Vests"
Array.
- List of class names used for the custom clothing.

Need to be vests attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Gloves"
Array.
- List of class names used for the custom clothing.

Need to be gloves attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Pants"
Array.
- List of class names used for the custom clothing.

Need to be pants/shorts attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Belts"
Array.
- List of class names used for the custom clothing.

Need to be belt attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Shoes"
Array.
- List of class names used for the custom clothing.

Need to be shoes attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Armbands"
Array.
- List of class names used for the custom clothing.

Need to be armbands attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.

### "Backpacks"
Array.
- List of class names used for the custom clothing.

Need to be backpacks attachments/items!
If the array only contains one item class name it the characters will always spawn with this item when "UseCustomClothing" is enabled
otherwise, the item will be selected randomly.


# Starting Gear
### "EnableStartingGear"
Bool.
- 0 = The player will spawn with the vanilla default gear.
- 1 = The player will spawn with the configured gear in this file.

### "UseUpperGear"
Bool.
- 0 = The "UpperGear" will not be used. Nothing from this list will spawn on the player character.
- 1 = The items from "UpperGear" will be added into the inventory of the player in his Upper inventory (shirt inventory).

### "UsePantsGear"
Bool.
- 0 = The "PantsGear" will not be used. Nothing from this list will spawn on the player character.
- 1 = The items from "PantsGear" will be added into the inventory of the player in his Pant inventory.

### "UseBackpackGear"
Bool.
- 0 = The "BackpackGear" will not be used. Nothing from this list will spawn on the player character.
- 1 = The items from "BackpackGear" will be added into the inventory of the player in his backpack inventory.

### "UseVestGear"
Bool.
- 0 = The "VestGear" will not be used. Nothing from this list will spawn on the player character.
- 1 = The items from "VestGear" will be added into the inventory of the player in his vest inventory.

### "UseVestGear"
Bool.
- 0 = The "VestGear" will not be used. Nothing from this list will spawn on the player character.
- 1 = The items from "VestGear" will be added into the inventory of the player in his vest inventory.

### "UsePrimaryWeapon"
Bool.
- 0 = The "PrimaryWeapon" will not be used. Player will not spawn with a primary weapon.
- 1 = The item defined at "PrimaryWeapon" will be added into the inventory of the player in his primary weapon slot.

### "UseSecondaryWeapon"
Bool.
- 0 = The "SecondaryWeapon" will not be used. Player will not spawn with a secondary weapon.
- 1 = The item defined at "SecondaryWeapon" will be added into the inventory of the player in his secondary weapon slot.

### "UpperGear"
Array. 
- List of class names used for the upper gear.

### "PantsGear"
Array. 
- List of class names used for the pants gear.

### "BackpackGear"
Array.
- List of class names used for the backpack gear.

### "VestGear"
Array.
- List of class names used for the vest gear.

### "PrimaryWeapon"
Array.
- Item that gets attached to the player's primary weapon slot. Need to be a Fire- or Meele Weapon like an Axe.

### "PrimaryWeaponAttachments"
Array.
- List of class names used for the primary weapon.
These items get attached to the player's primary weapon defined in the "PrimaryWeapon" config.
Make sure the attachments fit on this weapon. If this weapon is a melee weapon it cant fit any attachments!

### "SecondaryWeapon"
Array.
- Item that gets attached to the player's secondary weapon slot. Need to be a Fire- or Meele Weapon like an Axe.

### "SecondaryWeaponAttachments"
Array.
- List of class names used for the secondary weapon.
These items get attached to the player's secondary weapon defined in the "SecondaryWeapon" config.
Make sure the attachments fit on this weapon. If this weapon is a melee weapon it cant fit any attachments!

### "ApplyEnergySources"
Bool.
- 0 = Nothing happens here.
- 1 = All gear items with that the player character spawned get a V9 batterie when they can fit and need one.

### "SetRandomHealth"
Bool.
- 0 = All the gear items with that the player spawns are in a pristine condition.
- 1 = All the gear items with that the player character spawned are in a random condition.

# Spawn Selection:

### "EnableSpawnSelection"
Bool.
- 0 = Players will spawn randomly on the map like in vanilla.
- 1 = Players will be able to choose where to spawn on the map according the config done bellow.

### "SpawnSelectionScreenMenuID"
Integrer. The ID of the menu. If you are a modder, it will allow you to create custom menus.

### "SpawnOnTerritory"
Bool.
- 0 = Players can't respawn at their territories.
- 1 = You can respawn at your territory.

### "SpawnLocations"
Array. List of spawn locations

### "Name"
String. The name of the location

### "Positions"
Array. List of positions

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

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/SpawnSettings.json