![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Adding a circular safezone

First go to your server Expansion settings and open the SafezoneSettings.json file `\Profile (or config)\ExpansionMod\Settings`

![Server Expansion Settings Path](https://i.imgur.com/FXjTRN8.png)

Inside this file you should have all the already configured safezones for ChernaruPlus (the polygon safezone is a chernogorsk safezone for example, you maybe do not want that so think to replace them if you feel the need to).

![MissionSettings file](https://i.imgur.com/r8xjgjp.png)

Add the following lines (you have a picture to show how it should be done)

        {
            "MissionType": "ExpansionMissionEventAirdrop",
            "MissionPath": "$profile:ExpansionMod\\Missions\\NameOfMyCustomAirdrop.json"
        },

![Configured mission settings](https://i.imgur.com/TOaQuVC.png)

Now go to `\Profile (or config)\ExpansionMod\Missions` and create a file with the name you choosed to

![creating a json file](https://i.imgur.com/MLJNdqM.png)

## Configuring a airdrop

Inside your NameOfMyCustomAirdrop.json file you just created copy and paste the following lines :

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