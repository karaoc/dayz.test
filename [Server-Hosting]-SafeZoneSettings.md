Last updated the 20th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "Enabled"
Bool.
- 0 = Safezones will be turned off.
- 1 = Safezones will be enabled, however they still need to be configured.

### "EnableVehicleinvincibleInsideSafeZone"
Bool.
- 0 = Vehicles will take damage even when inside safezones.
- 1 = Vehicles can't be damaged inside safezones.

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

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/SafeZoneSettings.json