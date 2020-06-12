## Contents

- [Granting someone admin](#permissions)

- [Setting up permisisons](#permissions)

- [Setting up roles](#permissions)

- [Troubleshooting](#Troubleshooting)



## Granting someone admin

### 1. Getting the player ID

Firstly, make sure your admin logs are enabled ! How so ? By adding `-adminlog` in your server launch options.

**PICTURE HERE**

Now your server should generate new logs files in ADM format in your server profile (or config) folder

**PICTURE HERE**

You will be able to get Player IDs from this file. However to see the player id of someone, this player must have joined the server while this launch option was active !

Here is a example of what you should find :

**PICTURE HERE**

Now Remember this player ID and go to "YourDayZServer\Profile(or config)\PermissionFramework\Players\" you should see one or multiple files with players ids. Open the file with the player ID you saw in the logs. You should have something similar :

**PICTURE HERE**

Change "everyone" to "admin" and save. Now this player have the admin role ingame !

### 2. Granting the player admin role

## Setting up permisisons

_**Disclaimer**, this part is more advanced and does not require you to do the following steps to have a working server_


## Setting up roles

_**Disclaimer**, this part is more advanced and does not require you to do the following steps to have a working server_

## Troubleshooting

I only see vanilla vehicles in my spawnlist !

**PICTURE HERE**

Go inside your server config at YourDayZServer\Profile(or config)\ and delete the "CommunityOnlineTool" folder. It will force the admin tool to regenerate the list !