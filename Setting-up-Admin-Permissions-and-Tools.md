![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Contents

- [Granting someone admin](#granting-someone-admin)

- [Setting up permisisons](#setting-up-permisisons) TODO

- [Setting up roles](#setting-up-roles) TODO

- [Troubleshooting](#troubleshooting)



## Granting someone admin

### 1. Getting the player ID

Firstly, make sure your admin logs are enabled ! How so ? By adding `-adminlog` in your server launch options.

**PICTURE HERE**

Now your server should generate new logs files in ADM format in your server profile (or config) folder

**PICTURE HERE**

You will be able to get Player IDs from this file. However to see the player id of someone, this player must have joined the server while this launch option was active !

Here is a example of what you should find :

**PICTURE HERE**

### 2. Granting the player admin role

Now that you have found where to found the player ID, go to :

`YourDayZServer\Profile(or config)\PermissionFramework\Players\`

You should see one or multiple files with players IDs and open the file with the player ID you saw in the logs. You should have something similar :

**PICTURE HERE**

Change `everyone` to `admin` and save. Now this player have the admin role ingame ! _(you don't need to restart the server)_

## Setting up permisisons

_**Disclaimer**, this part is more advanced and does not require you to do the following steps to have a functionnal server and/or admin tool_

### 1. How do permissions works ?

0. None
1. It will gain the permission value of the next parent permission which is not inherit. So if you have `Admin.Player.Set` set to `INHERIT` and `Admin` set to `ALLOW` then `Admin.Player.Set` will be `ALLOW` but if you had `Admin.Player` set to `DISALLOW` as well then `Admin.Player.Set` is now `DISALLOW`.
2. Full access

### 2. How to add specific permissions to a user ?

## Setting up roles

_**Disclaimer**, this part is more advanced and does not require you to do the following steps to have a functionnal server and/or admin tool_

## Troubleshooting

##### I only see vanilla vehicles in my spawnlist !

**PICTURE HERE**

Go inside your server config at `YourDayZServer\Profile(or config)\` and delete the `CommunityOnlineTool` folder. It will force the admin tool to regenerate the list !

##### I can't open some menus in my admin tool !

Go inside your server config at `YourDayZServer\Profile(or config)\PermissionFramework\Roles\` and delete (or rename) the `everyone.txt` and `admin.txt` files. It will force the admin tool to regenerate the files and up to date!