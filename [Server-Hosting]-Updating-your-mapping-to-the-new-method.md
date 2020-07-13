![custom mapping](https://i.imgur.com/af8WSDT.jpg)

## Converting to the new format

You will need the software [Visual Studio Code](https://code.visualstudio.com/)

Once downloaded, create a empty file and paste all your SpawnObject lines inside it.
(you can also use [this software](https://github.com/virtyvoid/DayZPosConv) made by Def)

![SpawnObject list](https://i.imgur.com/pZV5OPQ.png)

Then press CTRL + H and write the following as shown in the picture (make sure to click on the small asterisk on the right or press ALT +R):

`SpawnObject\( "(.*)", "(.*)", "(.*)" \);`

`$1|$2|$3`

![Convert example](https://i.imgur.com/i5Cpvq8.png)

Click replace (or CTRL + ALT + ENTER) everything and Tada your mapping now follow the correct format !

![After converting](https://i.imgur.com/l91lFw9.png)

## Where to save ?

Now you want to save your file in your mission `\Expansion.MyWorldName\expansion\objects\` and save your mapping in .map format as shown in this picture.

![mapping directory](https://i.imgur.com/vjtsqJs.png)

## How to enable it ?

Now go inside your init.c and change `bool loadTraderObjects = false;` to `bool loadTraderObjects = true;`

![enabling mapping](https://i.imgur.com/PH7vIiI.png)

# Troubleshooting
If you are using a old expansion mission, please remove the following lines from your init.c file

![switch case to remove](https://i.imgur.com/rq5iGHj.png)