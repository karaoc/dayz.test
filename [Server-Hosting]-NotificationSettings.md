Last updated the 19th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "EnableNotification"
Bool. If set to 1, enable to notifications for everyone.

### "ShowPlayerJoinServer"
Bool. If set to 1, notify the player who joined the server.

### "JoinMessageType"
Integer. with 2 modes :

0. Will display the player joined message in the globalchat
1. Will display the player joined message in a notification

### "ShowPlayerLeftServer"
Bool. If set to 1, notify the player who left the server.

### "LeftMessageType"
Integer. with 2 modes :

0. Will display the player left message in the globalchat
1. Will display the player left message in a notification

### "ShowAirdropStarted"
Bool. If set to 1, will notify the player a airdrop just started.

### "ShowAirdropClosingOn"
Bool. If set to 1, will notify the player a airdrop is getting closer.

### "ShowAirdropDropped"
Bool. If set to 1, will notify the player a airdrop dropped the package.

### "ShowPlayerAirdropStarted"
Bool. If set to 1, will notify the player a airdrop called by a player just started.

### "ShowPlayerAirdropClosingOn"
Bool. If set to 1, will notify the player a airdrop called by a player is getting closer.

### "ShowPlayerAirdropDropped"
Bool. If set to 1, will notify the player a airdrop called by a player dropped the package.

### "ShowTerritoryNotifications"
Bool. If set to 1, will notify the player he entered/left a territory.

### "EnableKillFeed"
Bool. If set to 1, notify the player of whom got killed and how.

### "KillFeedMessageType"
Integer. with 2 modes :

0. Will display the player left message in the globalchat
1. Will display the player left message in a notification

### "EnableKillFeedDiscordMsg"
Bool. If set to 1, display the killfeed messages on a discord hook. A guide will be made later.

### "ShowVehicleDebugMarkers"
Bool.
- 0 = Will not do what 1 do and instead do nothing.
- 1 = Every vehicles on the map will have a marker displayed on the map on their position.

# Raw file

    {
        "EnableNotification": 1,
        "ShowPlayerJoinServer": 1,
        "JoinMessageType": 1,
        "ShowPlayerLeftServer": 1,
        "LeftMessageType": 1,
        "ShowAirdropStarted": 1,
        "ShowAirdropClosingOn": 1,
        "ShowAirdropDropped": 1,
        "ShowPlayerAirdropStarted": 1,
        "ShowPlayerAirdropClosingOn": 1,
        "ShowPlayerAirdropDropped": 1,
        "ShowTerritoryNotifications": 1,
        "EnableKillFeed": 1,
        "KillFeedMessageType": 1,
        "KillFeedFall": 1,
        "KillFeedCarHitDriver": 1,
        "KillFeedCarHitNoDriver": 1,
        "KillFeedCarCrash": 1,
        "KillFeedCarCrashCrew": 1,
        "KillFeedHeliHitDriver": 1,
        "KillFeedHeliHitNoDriver": 1,
        "KillFeedHeliCrash": 1,
        "KillFeedHeliCrashCrew": 1,
        "KillFeedBoatCrash": 1,
        "KillFeedBoatCrashCrew": 1,
        "KillFeedBarbedWire": 1,
        "KillFeedFire": 1,
        "KillFeedSpecialExplosion": 1,
        "KillFeedWeaponExplosion": 1,
        "KillFeedDehydration": 1,
        "KillFeedStarvation": 1,
        "KillFeedBleeding": 1,
        "KillFeedSuicide": 1,
        "KillFeedWeapon": 1,
        "KillFeedMeleeWeapon": 1,
        "KillFeedBarehands": 1,
        "KillFeedInfected": 1,
        "KillFeedAnimal": 1,
        "KillFeedKilledUnknown": 1,
        "KillFeedDiedUnknown": 1,
        "EnableKillFeedDiscordMsg": 1
    }