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

`-mod=@CF;@Community-Online-Tools;@DayZ-Expansion-;@DayZ-Expansion-Licensed-;@DayZ-Expansion-Vehicles-;@DayZ-Expansion-Core-`

### start.bat

If you are creating a local server (on your computer or on a local machine without omega manager for example) and don't know how or where to add this lines do the following.

Create a txt file and paste inside the file this config lines :

`@echo off
start DayZServer_x64.exe -config=serverDZ.cfg -port=2302 "-mod=@CF;@Community-Online-Tools;@DayZ-Expansion-;@DayZ-Expansion-Licensed-;@DayZ-Expansion-Vehicles-;@DayZ-Expansion-Core-" -profiles=.\ServerProfile -netlog`

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

After starting your server with the DayZ Expansion mod for the first time, the server will generate the ExpansionMod folder in your profile folder (sometimes also named "sc" or "config"), in this folder, all the DayZ Expansion related settings will be stored. If you want to toggle any part of DayZ Expansion go into the settings folder and open the file you want to modify. If you want to learn more about the server settings click [here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Server-settings).

![](https://i.imgur.com/4uEMoWi.png)

## Troubleshooting
#### Bad type 'StringLocaliser'

![](https://i.imgur.com/uFUrx8h.png)

Make sure you have the correct mods and up to date !

#### Addon ... Requires Addon 'JM_COT_Scripts'

![](https://i.imgur.com/CH9X0zx.png)

You are missing CF or Community-Online-Tools, make sure to have all the mods on your server !

#### Infinite loading screen, server frozen

For some reason, your ExpansionMod settings are broken. Revert the changes you have made or delete the folder. Some players reported that issue but infact it was just them not waiting. Please be sure it's a real issue and not you not waiting !

#### BattlEye initialization failed

The battle eye dll is missing from the battle eye folder of your server profile. A copy paste of this missing dll should do the job in most cases.

#### !!! String CORRUPTED - FIX OnStoreLoad() !!!

Your "storage_x" (x being a number) is using the vanilla storage format. Wipe this folder to use the Expansion storage format. This will wipe all player progression however.