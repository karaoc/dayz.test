![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Where to find the SafeZoneSettings

First go to your server Expansion settings and open the SafeZoneSettings.json file `\Profile (or config)\ExpansionMod\Settings`

![Server Expansion Settings Path](https://i.imgur.com/XfGvp38.png)

Inside this file you should have all the already configured safezones for ChernaruPlus. The already configured safezones are :
- One Circular SafeZone located at NEAF airstrip where the expansion trader will be located in the futur
- One Polygon SafeZone located at the town "Chernogorsk". Nothing is planned in this area.

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

- Currently circular safezones can only be **Type** of "1".
- **Center** is a array where you will need to specify the X Y Z coordinates of your safezone.
- **Radius** is the size in other words of your safezone.

## Adding a Polygon safezone

Add the following lines (you have a picture to show how it should be done)

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
    },

- Currently circular safezones can only be **Type** of "2".
- **Positions** is a array where you will need to specify the X Y Z coordinates of your safezone. Since this is a polygon, you need to add multiple positions like in this example to create a polygon shape safezone.
- **CenterPolygon** is a array where you will need to specify the X Y Z coordinates of the center your safezone. In case the Positions somehow fail to work, this will act as a failsafe.
- **RadiusPolygon** is the size in other words of your safezone. In case the Positions somehow fail to work, this will act as a failsafe.

Think to remove the , in }, at the last bracket. At the end of the page a couple of examples will be shown to help you if you are lost

## Some Examples

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
            },
            {
                "Type": 1,
                "Center": [
                    6200,
                    0,
                    9410
                ],
                "Radius": 250
            },
            {
                "Type": 1,
                "Center": [
                    4378.2,
                    0,
                    10951.1
                ],
                "Radius": 100
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
            },
            {
                "Type": 2,
                "Positions": [
                    [
                        4545,
                        0,
                        2181
                    ],
                    [
                        4298,
                        0,
                        2433
                    ],
                    [
                        4865,
                        0,
                        2945
                    ],
                    [
                        5000,
                        0,
                        2521
                    ]
                ],
                "CenterPolygon": [
                    6200,
                    0,
                    9410
                ],
                "RadiusPolygon": 250
            },
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
                    4378.2,
                    0,
                    10951.1
                ],
                "RadiusPolygon": 100
            }
        ]
    }