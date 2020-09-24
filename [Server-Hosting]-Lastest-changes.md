### Please think to update your server settings after each updates !

# Update 1.04.11XX

You can download the server setting files from this link : 

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings

## Mission files

Only the init.c changed (and the 109_lifetimes.xml but this is optionnal, if you don't use it, you don't need to worry)

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions/releases/

https://github.com/ExpansionModTeam/DayZ-Expansion-Missions

	class CustomMission: MissionServer
	{	
		Everything inside this class have been changed (for compatiblity with other mods)
	}

## SpawnSettings.json

Way too much changes, look at this page and copy paste ([click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-SpawnSettings#raw-file))

## BaseBuildingSettings.json

This setting was not renamed/removed but upgraded. You don't need to regenerate your file !

| Updated | Why |
|---|---|
| DismantleFlagRequireTools | You can now set this setting to -1 to only allow territory members to dismantle/destroy the flag |

To see the complete file please [click on this link](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-BaseBuildingSettings#raw-file)