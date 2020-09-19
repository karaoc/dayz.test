Last updated the 19th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "EnableNotification"
Bool.
- 0 = All the notifications will be disabled.
- 1 = Notifications will be enabled.

### "ShowPlayerJoinServer"
Bool.
- 0 = The "Player Joined the server" notification will not be displayed
- 1 = The "Player Joined the server" notification will be enabled

### "JoinMessageType"
Integrer.
- 0 = The notification will be displayed in the chat
- 1 = The notification will be displayed as a notification on the top left corner of your screen

### "ShowPlayerLeftServer"
Bool.
- 0 = The "Player left the server" notification will not be displayed
- 1 = The "Player left the server" notification will be enabled

### "LeftMessageType"
Integrer.
- 0 = The notification will be displayed in the chat
- 1 = The notification will be displayed as a notification on the top left corner of your screen

### "ShowAirdropStarted"
Bool.
- 0 = The notification when ever an airdrop event started will not be displayed
- 1 = Displays the notification when ever a airdrop event started.

### "ShowAirdropClosingOn"
Bool.
- 0 = The notification when ever an airdrop plane gets close to the drop location will not be displayed
- 1 = Displays the notification when ever a airdrop plane gets close to the drop location

### "ShowAirdropDropped"
Bool.
- 0 = The notification when ever an airdrop has been droped on the drop location will not be displayed
- 1 = Displays the notification when ever a airdrop has been droped on the drop location

### "ShowPlayerAirdropStarted"
Bool.
- 0 = The notification when ever a player calls an airdrop with an airdrop flare will not get displayed
- 1 = Displays the notification when a player calls an airdrop with an airdrop flare.

### "ShowPlayerAirdropClosingOn"
Bool.
- 0 = The notification when ever a player calls an airdorop with an airdrop flare and it gets close to the drop location will not be displayed
- 1 = Displays the notification when ever a player calls an airdorop with an airdrop flare and it gets close to the drop location

### "ShowPlayerAirdropDropped"
Bool.
- 0 = The notification when ever a player calls an airdorop with an airdrop flare and it has been droped on the drop location will not be displayed
- 1 = Displays the notification when ever a player calls an airdorop with an airdrop flare and it has been droped on the drop location

### "ShowTerritoryNotifications"
Bool.
- 0 = The notification when ever a player enters an territory will not be displayed
- 1 = Displays the notification when ever a player enters an territory

### "EnableKillFeed"
Bool.
- 0 = All the kill-feed notifications will be disabled
- 1 = Kill-feed will be enabled

### "KillFeedMessageType"
Bool.
- 0 = Kill-feed notification will be displayed in the chat
- 1 = Kill-feed notification will be displayed as a notification on the top left corner of your screen

### "KillFeedFall"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by fall damage
- 1 = Displays kill-feed notifications related to player deaths by fall damage

### "KillFeedCarHitDriver"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by an car hit with a driver in the car
- 1 = Displays kill-feed notifications related to player deaths by a car hit with a driver in the car

### "KillFeedCarHitNoDriver"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by an car hit with no driver in the car
- 1 = Displays kill-feed notifications related to player deaths by an car hit with no driver in the car

### "KillFeedCarCrash"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by an car crash.
- 1 = Displays kill-feed notifications related to player deaths by an car crash

### "KillFeedCarCrashCrew"
Bool.
- 0 = 
- 1 =

### "KillFeedHeliHitDriver"
Bool.
- 0 =
- 1 =

### "KillFeedHeliHitNoDriver"
Bool.
- 0 =
- 1 =

### "KillFeedHeliCrash"
Bool.
- 0 =
- 1 =

### "KillFeedHeliCrashCrew"
Bool.
- 0 =
- 1 =

### "KillFeedBoatCrash"
Bool.
- 0 =
- 1 =

### "KillFeedBoatCrashCrew"
Bool.
- 0 =
- 1 =

### "KillFeedBarbedWire"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by hit damage from barbed wires
- 1 = Displays kill-feed notifications related to player deaths by hit damage from barbed wires

### "KillFeedFire"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by hit damage from fireplaces
- 1 = Displays kill-feed notifications related to player deaths by hit damage from fireplaces

### "KillFeedWeaponExplosion"
Bool.
- 0 = Disables the display of kill-feed notifications related to player deaths by hit damage from a weapon explosion (granades, satchels..)
- 1 = Displays kill-feed notifications related to player deaths by hit damage from a weapon explosion

### "KillFeedDehydration"
Bool.
- 0 =
- 1 =

### "KillFeedStarvation"
Bool.
- 0 =
- 1 =

### "KillFeedBleeding"
Bool.
- 0 =
- 1 =

### "KillFeedSuicide"
Bool.
- 0 =
- 1 =

### "KillFeedWeapon"
Bool.
- 0 =
- 1 =

### "KillFeedMeleeWeapon"
Bool.
- 0 =
- 1 =

### "KillFeedBarehands"
Bool.
- 0 =
- 1 =

### "KillFeedInfected"
Bool.
- 0 =
- 1 =

### "KillFeedAnimal"
Bool.
- 0 =
- 1 =

### "KillFeedKilledUnknown"
Bool.
- 0 =
- 1 =

### "KillFeedDiedUnknown"
Bool.
- 0 =
- 1 =

### "EnableKillFeedDiscordMsg"
Bool.
- 0 =
- 1 =

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