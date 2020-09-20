Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "EnableParties"
Bool. If enabled, allow players to create parties.

### "MaxInParty"
Integrer. Maximum of players allowed in a single party. If <= 0, unlimited party size.

### "UseWholeMapForInviteList"
Bool. If enabled, you can invite everyone from anywhere regardless of the distance.

### "ShowPartyMembers3DMarkers"
Bool. If enabled, show a 3d marker above the head of your teammates.

### "DistanceForPartyMarkers"
Integrer. Distance in meters before the 3d marker fade out. Could not go over bubble network distance ~1000 m per default in DayZ

### "EnableQuickMarker"
Bool. If set to 1, allow players to use QuickMarkers (act like a ping ingame).

### "ShowDistanceUnderQuickMarkers"
Bool. If set to 1, show the distance between you and your quickmarker.

### "ShowNameOnQuickMarkers"
Bool. If set to 1, show the name of the user under the quickmarker.

# Raw file

    {
        "EnableParties": 1,
        "MaxMembersInParty": 10,
        "UseWholeMapForInviteList": 0,
        "EnablePartyMembersMapMarkers": 1,
        "EnablePartyMemberMarker": 1,
        "ShowDistanceUnderPartyMembersMarkers": 1,
        "ShowNameOnPartyMembersMarkers": 1,
        "EnableQuickMarker": 1,
        "ShowDistanceUnderQuickMarkers": 1,
        "ShowNameOnQuickMarkers": 1,
        "CanCreatePartyMarkers": 1
    }