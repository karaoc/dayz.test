![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Downloading the mods
- [CF](https://steamcommunity.com/workshop/filedetails/?id=1559212036)
- [Community-Online-Tools](https://steamcommunity.com/workshop/filedetails/?id=1564026768)
- [DayZ-Expansion](https://steamcommunity.com/sharedfiles/filedetails/?id=2116151222)
- [DayZ-Expansion-Licensed](https://steamcommunity.com/workshop/filedetails/?id=2116157322)

Download and install the mods listed above where your server is installed (as shown on the first picture). If you do not know how to get the mods follow the step 1 to 5 but don't go inside the Missions folder ! [Click me to see the tutorial page](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-offline-mode#getting-the-mission)

Inside each mods you should find a "key" folder with a bikey for each mods. Copy all this keys and paste them inside your keys folder (visible on the picture)

![Server root](https://i.imgur.com/OEaEuf8.png)

Make sure to launch the 4 mods with this command line if you don't use a panel : 

`-mod=@CF;@Community-Online-Tools;@DayZ-Expansion;@DayZ-Expansion-Licensed`

### start.bat

If you are creating a local server and don't know how or where to add this lines do the following.

Create a txt file and paste inside the file this config lines :

`@echo off
start DayZServer_x64.exe -config=serverDZ.cfg -port=2302 "-mod=@CF;@Community-Online-Tools;@DayZ-Expansion;@DayZ-Expansion-Licensed" -profiles=.\ServerProfile -netlog`

And save as MyName.bat !

Now all you have to do is to execute this bat file to launch your server 😃 

Make sure your bat file is inside your server folder as shown with the picture above !

## Mission files

Inside the mod "@DayZ-Expansion" take the mission files **that don't have COM in their name**.

![](https://i.imgur.com/yVtrGnb.png)

Copy and paste them inside your mpmission folder of your server. You should have this two new folders in this directory 👍 

![](https://i.imgur.com/wk7ezm6.png)

Now go back to the dayz server root and open your "**serverDZ.cfg**" config file (if you are on a web provider, make sure you can add custom mission or that you have expert mode enabled).

Inside this file, look for the template and change it to match this screenshot. You can choose to use the non Gloom mission if you want to. Gloom allow for better lighting visuals, this is the only difference !

![](https://i.imgur.com/eS46Rtu.png)

If you proceed with ChernarusPlusGloom mission file its important to set lightingConfig inside your server config file to 2. (by default this is the case)

## Server config

After starting your server with the DayZ Expansion mod for the first time, the server will generate the ExpansionMod folder in your profiles folder, in that folder all DayZ Expansion related settings and storage will be stored, if you want to toggle any part of DayZ Expansion proceeded into settings folder and open specific file you want to tweak. An overview of all the settings and what they do can be found [here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Server-settings)

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