Last updated the 22th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

This file has been updated with the latest update. I will do a complete documentation update later. But I still want to give you something to help you a bit. Here are the dev comments we have to explain these settings on our side : 

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
    New setting string array "VestGear" // String array for items that get spawned into the player's vest.
    New setting "PrimaryWeapon" // String for the item that gets spawned into the player's primary weapon slot.
    New setting "PrimaryWeaponAttachments" // String array for attachments that get attached to the player's primary weapon.
    New setting "SecondaryWeapon" // String for the item that gets spawned into the player's shoulder slot.
    New setting "SecondaryWeaponAttachments" // String array for attachments that get attached to the player's secondary weapon.
    New setting "ApplyEnergySources" // If enabled then all items that need a V9 batterie in players inventory a batterie attached.
    New setting "SetRandomHeath" // When enabled it will add random damage to the gear items with that a player spawn.

# StartingClothing:
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


# StartingGear
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
- 1 = All gear items with that the player character spawned get a V9 batterie when they can fit and need one,

### "SetRandomHealth"
Bool.
- 0 = All the gear items with that the player spawns are in a pristine condition.
- 1 = All the gear items with that the player character spawned are in a random condition.

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/SpawnSettings.json