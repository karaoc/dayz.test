Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

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
Bool.
- 0 = The player will not have a marker on his location.
- 1 = The player will have a marker on the map on his exact location. In short, a "you are here" marker.

### "ShowMapStats"
Bool.
- 0 = The player won't be able to know the XYZ position of a marker.
- 1 = The player will be able to know the XYZ position of a marker with the marker list of by holding SHIFT when his mouse will be hover a marker on the map.

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

### "ShowPartyMembersMapMarkers"
Bool. If enabled, show the player teammates position on the map.
- 0 = 
- 1 = 

### "ShowServerMarkers"
Bool. If enabled, show server map markers.
- 0 = 
- 1 = 

### "ShowNameOnServerMarkers"
Bool. If enabled, show the name of server map markers.
- 0 = 
- 1 = 

### "ShowDistanceOnServerMarkers"
Bool. If enabled, show the distance of server map markers.
- 0 = 
- 1 = 

### "ServerMarkers"
Array. Allow server owners to display server markers on the map. See [this tutorial](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-server-markers) for more explaination.

# Raw file

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
        "ServerMarkers": []
    }