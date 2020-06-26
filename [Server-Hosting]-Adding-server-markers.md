![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Where do you need to go ?

Go to `DayZServer\ServerProfile (or config)\ExpansionMod\Settings` and open the `MapSettings.json`

![Expansion Server Settings Path](https://i.imgur.com/Bste9wW.png)

Inside this file you should have something similar except you don't have the lines highlighted in white yet

![Map Settings File](https://i.imgur.com/3IPs6GC.png)

## How does it work ?

        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Hero Trader-Zone",
            "m_IconIndex": 5,
            "m_Color": -13710223,
            "m_Position": [
                11844.7,
                0,
                12466.8
            ]
        },

**REMOVE** the `,` from }, to the last marker config (look at the example)

#### m_IsPartyMarker

If set to 1,

#### m_Is3DMarker

If set to 1, your marker will be seen by everyone within the world. Be caution this can be quickly be a pain for players to have too much 3d markers displayed on their screen.

#### m_Text

This is where you will write the name of your marker !

#### m_IconIndex

What Icon will be used for the marker. Good news is, it's easy to know which one to use since they are in the correct order ingame :)

#### m_Color

The color of the marker, use this [this website to generate the color](https://thurston.pw/public/color.php) you want to apply on your marker !

#### m_Position

The position of the marker in XYZ coordinates.

## Some examples !

        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Hero Trader-Zone",
            "m_IconIndex": 5,
            "m_Color": -13710223,
            "m_Position": [
                11844.7,
                0,
                12466.8
            ]
        },
        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Bandit Trader-Zone",
            "m_IconIndex": 5,
            "m_Color": -1618884,
            "m_Position": [
                1127.14,
                0,
                2419.87
            ]
        },
        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Boat Trader",
            "m_IconIndex": 5,
            "m_Color": -13330213,
            "m_Position": [
                14355.7,
                0,
                13231.1
            ]
        },
        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Boat Trader",
            "m_IconIndex": 5,
            "m_Color": -13330213,
            "m_Position": [
                1755.13,
                0,
                2027.91
            ]
        },
        {
            "m_IsPartyMarker": 0,
            "m_Is3DMarker": 1,
            "m_Text": "Aircraft Trader",
            "m_IconIndex": 5,
            "m_Color": -13350562,
            "m_Position": [
                4971.66,
                0,
                2438.66
            ]
        }