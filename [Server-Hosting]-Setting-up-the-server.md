![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Downloading the mods
- [CF](https://steamcommunity.com/workshop/filedetails/?id=1559212036)
- [Community-Online-Tools](https://steamcommunity.com/workshop/filedetails/?id=1564026768)
- [DayZ-Expansion](https://steamcommunity.com/sharedfiles/filedetails/?id=2116151222)
- [DayZ-Expansion-Licensed](https://steamcommunity.com/workshop/filedetails/?id=2116157322)
- [DayZ-Expansion-Core](https://steamcommunity.com/sharedfiles/filedetails/?id=2291785308)
- [DayZ-Expansion-Vehicles](https://steamcommunity.com/sharedfiles/filedetails/?id=2291785437)

Download and install the mods listed above where your server is installed (as shown on the first picture). If you do not know how to get the mods follow the step 1 to 5 but don't go inside the Missions folder ! [Click me to see the tutorial page](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-offline-mode#getting-the-mission)

Inside each mods you should find a "key" folder with a bikey for each mods. Copy all this keys and paste them inside your keys folder (visible on the picture)

![Server root](https://i.imgur.com/OEaEuf8.png)

Make sure to launch the 4 mods with this command line if you don't use a panel : 

`-mod=@CF;@Community-Online-Tools;@DayZ-Expansion;@DayZ-Expansion-Licensed;@DayZ-Expansion-Vehicles;@DayZ-Expansion-Core`

### start.bat

If you are creating a local server (on your computer or on a local machine without omega manager for example) and don't know how or where to add this lines do the following.

Create a txt file and paste inside the file this config lines :

```
@echo off
start DayZServer_x64.exe -config=serverDZ.cfg -port=2302 "-mod=@CF;@Community-Online-Tools;@DayZ-Expansion;@DayZ-Expansion-Licensed;@DayZ-Expansion-Vehicles;@DayZ-Expansion-Core" -profiles=ServerProfile -netlog
```

And save as MyName.bat !

Now all you have to do is to execute this bat file to launch your server 😃 

Make sure your bat file is inside your server folder as shown with the picture above !

## Mission files

Download the lastest missions at [https://github.com/ExpansionModTeam/DayZ-Expansion-Missions/releases](https://github.com/ExpansionModTeam/DayZ-Expansion-Missions/releases) and extract the content of the zip file.

Take the mission files **who don't have COM in their name**.

![](https://i.imgur.com/yVtrGnb.png)

Copy and paste them inside your mpmission folder of your server. You should have this two new folders in this directory : 

![](https://i.imgur.com/4mLI7NV.png)

Now go back to the dayz server root directory and open your "**serverDZ.cfg**" config file (if you are on a web provider, make sure you can add custom mission or that you have expert mode enabled).

Inside this file, look for the template and change it to match this screenshot. You can choose to use the non Gloom mission if you want to. Gloom allow for better lighting visuals, this is the only difference !

![](https://i.imgur.com/eS46Rtu.png)

## Server config

After starting your server with the DayZ Expansion mod for the first time, the server will generate the ExpansionMod folder in your profile folder (sometimes also named "sc" or "config"), in this folder, all the DayZ Expansion related settings will be stored. If you want to toggle any part of DayZ Expansion go into the settings folder and open the file you want to modify. If you want to learn more about the server settings click [here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings).

![](https://i.imgur.com/4uEMoWi.png)

## Troubleshooting
#### Bad type 'StringLocaliser'

![](https://i.imgur.com/uFUrx8h.png)

Make sure you have the correct mods and up to date ! (in this case, it can't find CF)

#### Can't compile mission init script!

![](https://cdn.discordapp.com/attachments/717275490200715304/717995316921499658/unknown.png)

Your server is not loading Expansion, this is why you have this error.

#### Addon ... Requires Addon 'JM_COT_Scripts'

![](https://i.imgur.com/CH9X0zx.png)

You are missing Community-Online-Tools, make sure to have all the mods on your server !

#### Unknown types "ExpansionBaseBuilding"'

![](https://cdn.discordapp.com/attachments/717275490200715304/796749766687981608/unknown.png)

The Expansion mods are not up to date !

#### Infinite loading screen, server frozen

Check your logs and look for a error.
If you can find a error talking about a json error with a setting file. It usualy mean this file is broken (missing line for example). Revert your changes or fix the mistake manualy or with a json validator.

If you can't find any errors in the logs try the following : 
- Delete the folder "ExpansionMod" (in your "server profile" aka "config" aka "sc")
- Make sure you are loading a Expansion mission

##### Server not powerfull enough

Some server providers are not powerfull enough to run the **expansion custom mapping** and **building interiors**. You can disable this two features at your `server profile (in your "server profile" aka "config" aka "sc") => expansionmod => settings => GeneralSettings.json` and change this two settings from 1 to 0 if it's enabled.

##### ExpansionMod, Missions folder empty

If you `server profile (in your "server profile" aka "config" aka "sc") => expansionmod => missions` is empty, delete the "MissionSettings.json" from the settings folder

Please note: Some users thought their server was frozen while in fact it was the "!!! String CORRUPTED - FIX OnStoreLoad() !!!" issue.

##### The server can't find the mission (mpmission/expansion.mapname)

In this case, make sure the server is trying to open a mission with the correct name. A missing letter can change everything !

#### BattlEye initialization failed

The battlEye dll is missing from the battlEye folder of your server profile (also known as "config" or "sc"). A copy paste of this missing dll should do the job in most cases.

#### !!! String CORRUPTED - FIX OnStoreLoad() !!!

Your "storage_x" (x being a number) is using the vanilla storage format. Wipe this folder to use the CF storage format. This will wipe all player progression however.