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

TODO

#### m_Is3D

If set to 1, your marker will be seen by everyone within the world. Be caution this can be quickly be a pain for players to have too much 3d markers displayed on their screen.

#### m_Text

This is where you will write the name of your marker !

#### m_IconName

What Icon will be used for the marker. Good news is, it's easy to know which one to use since they are in the correct order ingame :)

    "Arrow",
    "Error",
    "Infected 1",
    "Infected 2",
    "Territory",
    "Drip",
    "Ear",
    "Fireplace",
    "Hook",
    "Info",
    "Knife",
    "Marker",
    "Menu",
    "Moon",
    "Pen",
    "Persona",
    "Pill",
    "Star",
    "Sun",
    "Thermometer",
    "Book 1",
    "Book 2",
    "Ellipse",
    "Grab",
    "Open Hand",
    "Map",
    "Note",
    "Orientation",
    "Radio",
    "Shield",
    "Snow",
    "Group",
    "Infected 2",
    "Vehicle Crash",
    "Airdrop",    
    "Car",                    
    "Deliver",            
    "Map Marker",        
    "Radiation",
    "Trader",            
    "Water",            
    "Infected",
    "Skull",
    "Helicopter",
    "Base",
    "Boat",
    "Fishing",
    "Map Marker 2",
    "Water 2",
    "Questionmark",
    "Person",
    "Hearth",
    "Eye",
    "Claw",
    "Bear",
    "Skull 2",
    "Skull 3",    
    "Tent"

#### m_Color

The color of the marker, use this [this website to generate the color](https://thurston.pw/public/color.php) you want to apply on your marker !

#### m_Position

The position of the marker in XYZ coordinates.

## Some examples !

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