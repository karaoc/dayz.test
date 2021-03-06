![airdrop](https://i.imgur.com/TZpLHYq.png)

## Adding a airdrop

First go to your server Expansion settings and open the MissionSettings.json file `\Profile (or config)\ExpansionMod\Settings`

![Server Expansion Settings Path](https://i.imgur.com/FXjTRN8.png)

Inside this file you should have all the already configured airdrops for ChernaruPlus. The `TimeBetweenMissions` is in **miliseconds** !

![MissionSettings file](https://i.imgur.com/i5Elt1u.png)

Add the following lines (you have a picture to show how it should be done)

```
        {
            "MissionType": "ExpansionMissionEventAirdrop",
            "MissionPath": "$profile:ExpansionMod\\Missions\\NameOfMyCustomAirdrop.json"
        },
```

![Configured mission settings](https://i.imgur.com/svi2PSD.png)

Now go to `\Profile (or config)\ExpansionMod\Missions` and create a file with the name you choosed to

![creating a json file](https://i.imgur.com/xW4mdto.png)

## Configuring a airdrop

Inside your **NameOfMyCustomAirdrop.json** file you have just created copy and paste the following lines :

```
{
    "Enabled": 1,
    "Weight": 21.0,
    "MissionMaxTime": 1200,
    "MissionName": "Name_of_my_mission",
    "Difficulty": 0,
    "Objective": 0,
    "Reward": "",
    "ShowNotification": 1,
    "Height": 750.0,
    "Speed": 25.0,
    "Container": "Random",
    "DropLocation": {
        "x": 1000.0,
        "z": 0.0,
        "Name": "Name to display",
        "Radius": 100.0
    },
    "Loot": [],
    "Infected": [],
    "ItemCount": 0,
    "InfectedCount": -1
}
```

### "Weight"
How important is this airdrop, the bigger the number is, the more likely it will be picked. If you want this airdrop to be rare take a smaller number compared to the other missions !

### "MissionMaxTime"
How long this airdrop could stay on the map until it's destroyed by zombies (despawn)? It's in **seconds**.

### "MissionName"
String. This is the "id" of the mission, it need to be unique. We recommend you to use the following naming convention: `Type_Location`. For example: `Medical_Kamenka`.

### "Difficulty"
**Unused** at the moment. Keep it at 0

### "Objective"
**Unused** at the moment. Keep it at 0

### "Reward"
String. **Unused** at the moment. Keep it empty

### "ShowNotification"
Bool.
- 0: this airdrop will not send any notifications to the players
- 1: this airdrop will notify players with a notification (only if notifications are not disabled in NotificationSettings.json ! )

### "Height"
Float. The altitude the plane will fly at. (his **Y** position in other words)

### "Speed"
Float. The speed of the plane.

### "Container"
String. What type of airdrops will be spawned : 
* Random

### "DropLocation"
Array.
- X: The position X
- Z: The position Z (in DayZ, Y is the up/down axis)
- Name: The name of your airdrop, this is the name you will see in the notification about the airdrop. `"Airdrop have been dropped at MyNameHere"`
- Radius: the drop radius based on the x/z position you gave. If you want the airdrop to land at the exact position, just set this setting to 0.

```
    "DropLocation": {
        "x": 1000.0,
        "z": 0.0,
        "Name": "MyNameHere",
        "Radius": 100.0
    },
```

### "Loot"
What loot could spawn inside the airdrop. You have to give the Name of the Classname, his chance of spawning (1.00 = 100%) and his attachements if you want it to spawn with items attached to it. Please make sure the last `}` of the loot list doesn't have the `,` in `},` like in the example !

### "Infected"
A list of AI that will spawn around the airdrop once landed. Zombies or animals for example.

### "ItemCount"
The amount of items the airdrop will have in it

### "InfectedCount"
The amount of Zombies around the airdrop
