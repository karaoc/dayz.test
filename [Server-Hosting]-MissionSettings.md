Last updated the 19th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "Enabled"
Bool.
- 0 = All the missions will be disabled.
- 1 = It will enable missions, currently only airdrop missions are available but more are planned in the futur.

### "TimeBetweenMissions"
Integrer. Time in milliseconds before a new mission start

### "MinMissions"
Integrer. Minimum mission allowed at once. The number should not be greater than "MaxMissions".

### "MaxMissions"
Integrer. Maximum mission allowed at once.

### "MinPlayersToStartMissions"
Integrer. Minimum required of players to start a mission.

### "Missions"
Array. List the missions configured on the server. Currently only used for [airdrops](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-custom-airdrops).

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/MissionSettings.json