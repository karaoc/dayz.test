Last updated the 19th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "EnableMap"
Bool.
- 0 = Will use the vanilla map UI (white map)
- 1 = Will use the Expansion map UI (colored map)

### "UseMapOnMapItem"
Bool.
- 0 = The default vanilla map UI will be used when using the map item "open map" action.
- 1 = The Expansion map UI will be used when using the map item "open map" action.

### "ShowPlayerPosition"
Integrer.
- 0 = The player will not have a marker on his location.
- 1 = The player will have a marker on the map on his exact location. In short, a "you are here" marker.
- 2 = The player will have a marker on the map on his exact location if the player have a compass in his inventory or his hands.

### "ShowMapStats"
Bool.
- 0 = The player won't be able to know the XYZ position of a marker.
- 1 = The player will be able to know the XYZ position of a marker with the marker list of by holding SHIFT when his mouse will be hover a marker on the map.

### "NeedPenItemForCreateMarker"
Bool.
- 0 = The player don't need a Pen to create markers on the map.
- 1 = The player need a Pen in his inventory to create markers on the map.

### "CanCreateMarker"
Bool.
- 0 = The player won't be able to create any markers.
- 1 = Allow the player to create markers on the map.

### "CanCreate3DMarker"
Bool. Require "CanCreateMarker" to be enabled (set to 1)
- 0 = The player will not be able to create 3D markers.
- 1 = Allow the player to create 3D markers on the map.

### "CanOpenMapWithKeyBinding"
Bool.
- 0 = The player will have to open a physical item map to see the map.
- 1 = The player can open the map with a keybind instead of interacting with the physical map ("Open map" action).

### "EnableHUDGPS"
Bool. 
- 0 = The player will be only able to open the map with M
- 1 = The player will be able to enabled the GPS HUD by Holding N and to switch modes by tapping N. He will also be able to open the map with M

### "NeedGPSItemForKeyBinding"
Bool.
- 0 = You don't need the GPS item to open the map (M) or the GPS UI (hold N and tap N to switch modes)
- 1 = You need the physical GPS item to open the map (M) or the GPS UI (hold N and tap N to switch modes)

### "NeedMapItemForKeyBinding"
Bool.
- 0 = You don't need the map item to open the map (M)
- 1 = You need the physical map item to open the map (M)

### "EnableServerMarkers"
Bool.
- 0 = All the server markers will be disabled and invisible on the map.
- 1 = The server markers will be enabled and visible.

### "ShowNameOnServerMarkers"
Bool.
- 0 = All the server markers won't have a name.
- 1 = All the server markers will display the name they have configured.

### "ShowDistanceOnServerMarkers"
Bool.
- 0 = The distance under the server markers won't be displayed.
- 1 = The distance under the server markers will be displayed.

### "ServerMarkers"
Array. Allow server owners to display server markers on the map. See [this tutorial](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-server-markers) for more explaination.

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/MapSettings.json