![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Where to find the SafeZoneSettings

First go to your server Expansion settings and open the SafeZoneSettings.json file `\Profile (or config)\ExpansionMod\Settings`

![Server Expansion Settings Path](https://i.imgur.com/XfGvp38.png)

Inside this file you should have all the already configured safezones for ChernaruPlus. The already configured safezones are :
- One Circular SafeZone located at NEAF airstrip where the expansion trader will be located in the futur
- One Polygon SafeZone located at the town "Chernogorsk". Nothing is planned in this area.

![SafeZoneSettings file](https://i.imgur.com/W7XW2mQ.png)

    {
        "Enabled": 0,
        "EnableVehicleinvincibleInsideSafeZone": 1,
        "FrameRateCheckSafeZoneInMs": 5000,
        "CircleZones": [
            {
                "Type": 1,
                "Center": [
                    11849.6,
                    0,
                    12471.6
                ],
                "Radius": 500
            }
        ],
        "PolygonZones": [
            {
                "Type": 2,
                "Positions": [
                    [
                        6345,
                        0,
                        2181
                    ],
                    [
                        6198,
                        0,
                        2433
                    ],
                    [
                        6565,
                        0,
                        2945
                    ],
                    [
                        7000,
                        0,
                        2521
                    ]
                ],
                "CenterPolygon": [
                    6561.09,
                    0,
                    2540.71
                ],
                "RadiusPolygon": 439.351
            }
        ]
    }

### "Enabled"
Bool. Enable Safezone when set to 1.

### "EnableVehicleinvincibleInsideSafeZone"
Bool. When enabled, Vehicle damage is disabled.

### "FrameRateCheckSafeZoneInMs"
Integrer. How often in ms the server need to check if the player is inside a Safezone.

### "CircleZones"
Array. 
- Type: Tell which type of safezone it is (circular or polygon) by indicating 1 or 2. For a CircleZones it's 1
- Center: where the zone should be on the map
- Radius: Size of the zone

### "PolygonZones"
Array.
- Type: Tell which type of safezone it is (circular or polygon) by indicating 1 or 2. For a PolygonZones it's 2
- Positions: A array of positions to draw this polygon.
- CenterPolygon: where the zone should be on the map
- RadiusPolygon: Size of the zone

## Adding a circular safezone

Add the following lines (you have a picture to show how it should be done)

        {
            "Type": 1,
            "Center": [
                11849.6,
                0,
                12471.6
            ],
            "Radius": 500
        },

Currently circular safezones can only be **Type** of "1".
**Center** is a array where you will need to specify the X Y Z coordinates of your safezone.
**Radius** is the size in other words of your safezone.