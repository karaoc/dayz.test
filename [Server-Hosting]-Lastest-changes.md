# TESTING GROUND PAGE - THIS PAGE IS NOT FINAL


### Please think to update your server settings after each updates !

# Update 1.04.xxxx

## BaseBuildingSettings.json

The following settings got their name changed !

| Before | After | Why |
|---|---|---|
| CanDismantleFlag | DismantleFlagRequireTools | The name was not easy to understand |
| EnableSimpleFlagBuilding | SimpleTerritory | The name was not easy to understand |
| AddFlagItem | AutomaticFlagOnCreation | The name was not easy to understand |

To see the complete file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings#raw-file)

## GeneralSettings.json

The following settings got removed from this file and got moved in another file (MapSettings.json)

| Removed | Why |
|---|---|
| EnableHUDGPS | Moved to MapSettings.json to make it easier for new users to find what they are looking for |
| NeedGPSItemForKeyBinding | Moved to MapSettings.json to make it easier for new users to find what they are looking for |
| NeedMapItemForKeyBinding | Moved to MapSettings.json to make it easier for new users to find what they are looking for |

To see the complete file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings#raw-file)

## MapSettings.json

| Added | Why |
|---|---|
| EnableHUDGPS | Moved to MapSettings.json to make it easier for new users to find what they are looking for | 
| NeedGPSItemForKeyBinding | Moved to MapSettings.json to make it easier for new users to find what they are looking for | 
| NeedMapItemForKeyBinding | Moved to MapSettings.json to make it easier for new users to find what they are looking for | 

| Removed | Why |
|---|---|
| CanCreatePartyMarkers | Moved to PartySettings.json to make it easier for new users to find what they are looking for | 
| ShowPartyMembersMapMarkers | Moved to PartySettings.json to make it easier for new users to find what they are looking for | 

The following setting got renamed

| Before | After | Why |
|---|---|---|
| ShowServerMarkers | EnableServerMarkers | To follow the same naming format used | 

To see the complete file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings#raw-file)

## PartySettings.json

The following settings got their name changed !

| Before | After | Why |
|---|---|---|
| MaxInParty | MaxMembersInParty | Goal is to make this setting easier to understand for new users | 
| ShowPartyMembers3DMarkers | ShowPartyMembersMapMarkers | To follow the same naming format used | 
| AddFlagItem | AutomaticFlagOnCreation | To follow the same naming format used | 

To see the complete file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings#raw-file)