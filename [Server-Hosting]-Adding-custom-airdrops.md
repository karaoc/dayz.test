![airdrop](https://i.imgur.com/TZpLHYq.png)

## Adding a airdrop

First go to your server Expansion settings and open the MissionSettings.json file `\Profile (or config)\ExpansionMod\Settings`

![Server Expansion Settings Path](https://i.imgur.com/FXjTRN8.png)

Inside this file you should have all the already configured airdrops for ChernaruPlus. The `TimeBetweenMissions` is in miliseconds !

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

Inside your airdrop.json file you just created copy and paste the following lines :

        {
        "Enabled": 1,
        "Weight": 150,
        "MissionMaxTime": 1200,
        "MissionName": "Name_of_my_mission",
        "Difficulty": 0,
        "Objective": 0,
        "Reward": "",
        "ShowNotification": 1,
        "Height": 750,
        "Speed": 25,
        "Container": "ExpansionAirdropContainer_Military",
        "DropLocation": {
            "x": 5043,
            "y": 2505,
            "Name": "Name to display",
            "Radius": 100
        },
        "Loot": [
        {
            "Name": "AK74",
            "Attachments": [
                "KobraOptic",
                "AK_WoodHndgrd",
                "AK74_WoodBttstck"
            ],
            "Chance": 0.30
        },
        {
            "Name": "Bear_Pink",
            "Attachments": [],
            "Chance": 0.70
        },

        ],
        "Infected": [
            "ZmbM_HermitSkinny_Base",
            "ZmbM_HermitSkinny_Beige",
            "ZmbM_HermitSkinny_Black",
            "ZmbM_HermitSkinny_Green",
            "ZmbM_HermitSkinny_Red",
        ],
        "ItemCount": 5,
        "InfectedCount": 10
    }

### "Weight"
How important is this airdrop, the bigger the number is, the more likely it will be picked. If you want this airdrop to be rare take a smaller number compared to the other airdrops !

### "MissionMaxTime"
How long this airdrop could stay on the map until it despawn? It's in seconds.

### "MissionName"
Currentlty useless since missions are only used for airdrops but will be used in the futur to create multiple categories for missions.

### "Difficulty"
Unused at the moment. Keep it at 0

### "Objective"
Unused at the moment. Keep it at 0

### "Reward"
Unused at the moment. Keep it empty

### "ShowNotification"
If set to 1, this specific airdrop will notify players with a notification if notifications are not disabled in NotificationSettings.json !

### "Height"
The altitude the plane will fly at.

### "Speed"
The speed of the plane.

### "Container"
What container will be used for the airdrop. By default you can choose between :
* ExpansionAirdropContainer_Military
* ExpansionAirdropContainer_Basebuilding
* ExpansionAirdropContainer_Medical
* ExpansionAirdropContainer