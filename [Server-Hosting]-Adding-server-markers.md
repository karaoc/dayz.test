![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Where do you need to go ?

Go to `DayZServer\ServerProfile (or config)\ExpansionMod\Settings` and open the `MapSettings.json`

![Expansion Server Settings Path](https://i.imgur.com/Bste9wW.png)

Inside this file you should have something similar except you don't have the lines highlighted in white yet

![Map Settings File](https://i.imgur.com/A1V5Bog.png)

## How does it work ?

    {
        "m_UID": "MyUniqueID101",
        "m_Visibility": 6,
        "m_Is3D": 1,
        "m_Text": "My Marker Name",
        "m_IconName": "IconName",
        "m_Color": -13710223,
        "m_Position": [
            X,
            Y,
            Z
        ]
    },

**REMOVE** the `,` from `},` to the last marker config (look at the [example](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-server-markers#some-examples-) at the end of the page)

#### m_UID

The UID is the unique identity of a marker, this mean it need a unique ID to be valid. This ID can have numbers or letters.

#### m_Visibility

- 0 = Not visible.
- 2 = Visible on the World (If "m_Is3D" is set to 1, you should probably put "m_Visibility" to 2).
- 4 = Visible on the Map only.
- 6 = Visible on the Map and on the World (If "m_Is3D" is set to 1, you should probably put "m_Visibility" to 2).

#### m_Is3D

If set to 1, your marker will be seen by everyone within the world. Be caution this can be quickly be a pain for players to have too much 3d markers displayed on their screen.

#### m_Text

This is where you will write the name of your marker !

#### m_IconName

What Icon will be used for the marker. Good news is, it's easy to know which one to use since they are in the correct order ingame :)

    "Arrow"
    "Error"
    "Airdrop"
    "Car"
    "Deliver"
    "Radiation"
    "Trader"
    "Water 1"
    "Water 2"
    "Infected 1"
    "Infected 2"
    "Skull 1"
    "Skull 2"
    "Skull 3"
    "Helicopter"
    "Base"
    "Boat"
    "Fishing"
    "Territory"
    "Bear"
    "Claw"
    "Drip"
    "Ear"
    "Eye"
    "Fireplace"
    "Heart"
    "Hook"
    "Info"
    "Knife"
    "Map"
    "Marker"
    "Map Marker"
    "Orientation"
    "Menu"
    "Pen"
    "Persona"
    "Pill"
    "Questionmark"
    "Moon"
    "Star"
    "Sun"
    "Ellipse"
    "Tent"
    "Thermometer"
    "Book 1"
    "Book 2"
    "Note"
    "Grab"
    "Open Hand"
    "Radio"
    "Shield"
    "Snow"
    "Group"
    "Vehicle Crash"
    "Animal Skull"
    "Apple"
    "Apple Core"
    "Arrows"
    "Axe"
    "Backpack"
    "Bandage"
    "Batteries"
    "Berries"
    "Kitchen Knife Big"
    "Binoculars"
    "Bolt"
    "Bonfire"
    "Bottle"
    "Bow"
    "Broken Lighter"
    "Can Of Beans Big"
    "Can Of Beans Small"
    "Car Keys"
    "Carrot"
    "Chain Saw"
    "Chicken"
    "Chocolate"
    "Cigarets"
    "Cloth"
    "Compass"
    "Corn"
    "Crowbar"
    "Cow"
    "Dinosaur Skull"
    "Dry Wood"
    "Eatable Flowers"
    "Electrical Tape"
    "Empty Can"
    "Fish"
    "Flare"
    "Flare Gun"
    "Flare Gun Ammo"
    "Flashlight"
    "Fox"
    "Frying Pan"
    "Gas"
    "Gas Mask"
    "Golf Club"
    "Goose"
    "Grenade"
    "Guitar"
    "Gun"
    "Gun Bullets"
    "Hammer"
    "Herbal Medicine"
    "Home Made Grenade"
    "Human Skull"
    "Insect"
    "Kitchen Knife"
    "Ladder"
    "Lantern"
    "Lighter"
    "Machette"
    "Paper Map"
    "Matches"
    "Medic Box"
    "Mushrooms"
    "Nails"
    "Paper"
    "Pills"
    "Pipe Wrench"
    "Powder"
    "Pumpkin"
    "Rabbit"
    "Raccon"
    "Radio"
    "Rat"
    "Rock 1"
    "Rock 2"
    "Rope"
    "Saw"
    "Scrap Metal"
    "Screwdriver"
    "Shotgun"
    "Shotgun Bullets"
    "Shovel"
    "Soda"
    "Tent Small"
    "Walkie Talkie"
    "Water Jug"
    "Wild Pork"
    "Worms"

#### m_Color

The color of the marker, use this [this website to generate the color](https://thurston.pw/public/color.php) you want to apply on your marker !

**Warning** Values you have to enter have to be between 1 and 255. 0 is not a valid option !

- A: Opacity from 1 (can't be seen) to 255 (very visible, opaque)
- R: Red
- G: Green
- B: Blue

You can use [this website to generate the RGBA color](https://htmlcolors.com/rgba-color), however watch out this website generate the A value from 0 to 1 instead of 255 !

#### m_Position

The position of the marker in XYZ coordinates.

## Some examples !

    {
        "EnableMap": 1,
        "UseMapOnMapItem": 1,
        "ShowPlayerPosition": 1,
        "ShowMapStats": 1,
        "CanCreateMarker": 1,
        "CanCreate3DMarker": 1,
        "CanOpenMapWithKeyBinding": 1,
        "EnableHUDGPS": 1,
        "NeedGPSItemForKeyBinding": 1,
        "NeedMapItemForKeyBinding": 1,
        "EnableServerMarkers": 1,
        "ShowNameOnServerMarkers": 1,
        "ShowDistanceOnServerMarkers": 1,
        "ServerMarkers": [
            {
                "m_UID": "Green Mountain Trader",
                "m_Visibility": 6,
                "m_Is3D": 1,
                "m_Text": "Green Mountain Trader",
                "m_IconName": "Trader",
                "m_Color": -13710223,
                "m_Position": [
                    3697,
                    402.13,
                    5987
                ]
            },
            {
                "m_UID": "Eastwatch Trader",
                "m_Visibility": 6,
                "m_Is3D": 1,
                "m_Text": "Eastwatch Trader",
                "m_IconName": "Trader",
                "m_Color": -13710223,
                "m_Position": [
                    14303,
                    5,
                    13275
                ]
            },
            {
                "m_UID": "Black Market Trader",
                "m_Visibility": 6,
                "m_Is3D": 1,
                "m_Text": "Black Market Trader",
                "m_IconName": "Trader",
                "m_Color": -13710223,
                "m_Position": [
                    1362,
                    345,
                    9310
                ]
            }
        ]
    }