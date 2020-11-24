### Please think to update your server settings after each updates !

# Update 1.05.1155

You can download the server setting files from this link : 

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings

You can see all the changes in the server settings with this link: 

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/commit/a0fcfb238aba9d245f19ab6b31005e7e6b44f786

## Mission files

Only minor changes to the mission files. Update them if you want to but **it's not required**.

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions/releases/

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions

## RaidSettings.json

This setting should be placed at the very end of the file after "SafeProjectileDamageMultiplier"

| Added| Why |
|---|---|
| BaseBuildingRaidMode | Allow servers to balance a bit more raiding by only allowing raiding on doors/gates (and windows if they want to) |

- 0 = every basebuilding elements can be raided
- 1 = only doors/gates
- 2 = only doors/gates/windows

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-RaidSettings)

## BaseBuildingSettings.json

This setting **doesn't require you to regenerate this file**, if you are not interested in the mode "2" of this setting you won't have to do anything

| Updated | Why |
|---|---|
| EnableFlagMenu | Idea is to give more choices to how to use the territory system for the servers. |

- 0 = Disabled
- 1 = Default, you can choose your flag and create a territory
- 2 = You can only create a territory. The flag on the flag pole will be your flag and you won't be able to change it.

To see the complete documentation about this file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings)