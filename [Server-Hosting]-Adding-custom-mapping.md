![custom mapping](https://i.imgur.com/af8WSDT.jpg)

# Requirements:
First, make sure to have Expansion COM installed and functional
[https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-offline-mode](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-offline-mode)

# Placing Objects:
Once in game in the offline mode you are able to bring up the COM menu by pressing "U" on your keyboard.
The menu will show up on the right side of your screen:
![COT Menu](https://i.imgur.com/a9LJ2W8.jpg)

Click on the first menu button to bring up the Items and Objects spawner menu:
![COT Menu](https://i.imgur.com/7fSgnx5.jpg)

Select the object you want to spawn in the list and doubleclick with the left mouse button on the position after that
to place the object on that position:
![COT Menu](https://i.imgur.com/K02pMDU.jpg)

You can manage and change your placed object in the Object Info menu:
![COT Menu](https://i.imgur.com/VduEw2o.jpg)

# Export:
Once you have finished the placement of your objects you can export your work with a simple click on the Object Info menu button called "Export":
![COT Menu](https://i.imgur.com/hqS0Ugt.jpg)

This will copy all the lines to your clipboard.

Make sure you save your work if you want to keep it for later use by pressing the Save button!
This will create a file on your local drive with all the required information
(Example: C:\Users\username\Documents\DayZ\CommunityOfflineMode\Scenes\latest.json) so it can be used again in offline mode.

# Import:
Once you have exported all the lines to your clipboard you will need to import these to your Expansion.WOLDNAME mission to so they work on your server.
For this you need to create a new [.MAP](https://en.wikipedia.org/wiki/MAP_(file_format)) file in the directory:
Expansion.WORLDNAME\expansion\objects and paste in the exported lines. 
**The file can be named to what ever you want as the system will load every correct .map file that is in that folder!**

# Mission Setup:
By default the objects spawn system within the mission is disabled. 
To make sure that the mission spawns all objects you need to make sure you allow that by setting a boolean to true within the **Expansion.WORLDNAME\init.c** (also work for ExpansionCOM missions) for  file called:

`bool loadTraderObjects = true;`

If this line is set to false for you set it to true so the mission loads all the .map files.

# Troubleshooting
If you are using a old expansion mission, please remove the following lines from your init.c file

![switch case to remove](https://i.imgur.com/rq5iGHj.png)