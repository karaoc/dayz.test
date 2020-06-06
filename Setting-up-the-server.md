# Downloading the mods
- [CF](https://steamcommunity.com/workshop/filedetails/?id=1559212036)
- [Community-Online-Tools](https://steamcommunity.com/workshop/filedetails/?id=1564026768)
- [DayZ-Expansion](https://steamcommunity.com/sharedfiles/filedetails/?id=2116151222)
- [DayZ-Expansion-Licensed](https://steamcommunity.com/workshop/filedetails/?id=2116157322)

Install them on your server. You should get a similar result. If you do not know how to get the mods follow the step 1 to 5 but don't go inside folder ! [Click me to see the tutorial page](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-offline-mode#getting-the-mission)

![Server root](https://i.imgur.com/OEaEuf8.png)

# Mission files

Inside the mod "@DayZ-Expansion" take the mission files **that don't have COM in their name**.

![](https://i.imgur.com/yVtrGnb.png)

Copy and paste them inside your mpmission folder of your server. You should have this two new folders in this directory 👍 

![](https://i.imgur.com/wk7ezm6.png)

Now go back to the dayz server root and open your "serverDZ.cfg" config file (if you are on a web provider, make sure you can add custom mission or that you have expert mode enabled).

Inside this file, look for the template and change it to match this screenshot. You can choose to use the non Gloom mission if you want to. Gloom allow for better lighting visuals, this is the only difference !

![](https://i.imgur.com/eS46Rtu.png)

If you proceed with ChernarusPlusGloom mission file its important to set lightingConfig inside your server config file to 2. (by default this is the case)

# Server config

After starting your server with the DayZ Expansion mod for the first time, the server will generate the ExpansionMod folder in your profiles folder, in that folder all DayZ Expansion related settings and storage will be stored, if you want to toggle any part of DayZ Expansion proceeded into settings folder and open specific file you want to tweak. An overview of all the settings and what they do can be found [here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Server-settings)

