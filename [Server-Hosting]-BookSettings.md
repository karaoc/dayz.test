Last updated the 19th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "EnableBook"
Bool.
- 0 = The book will be disabled.
- 1 = The book will be enabled, the book is used for party and territory management but also for server rules and informations.

### "EnableStatusTab"
Bool. 
- 0 = This feature will be removed from the book
- 1 = The status tab will be available. The status tab contains character info like health, hunger/thirst values, etc. 

### "EnablePartyTab"
Bool.
- 0 = This feature will be removed from the book.
- 1 = The party tab will be available allowing players to manage and creating parties and invite players. You can tweak parties in the PartySettings.json

### "EnableServerInfoTab"
Bool.
- 0 = This feature will be removed from the book.
- 1 = A server info page will be available allowing you to provide a description of your server, buttons to redirect the player to your discord, forum or other places.

### "EnableServerRulesTab"
Bool.
- 0 = This feature will be removed from the book.
- 1 = The server rules tab will be available. This page allow servers to display their rules

### "EnableTerritoryTab"
Bool. If enabled, the territory tab will be available.
- 0 = This feature will be removed from the book.
- 1 = The territory tab will be available allowing players to manage their territories and invite players. You can tweak territories in the TerritorySettings.json

### "ShowServerSettings"
Bool. Require "EnableServerInfoTab" to be enabled (set to 1)
- 0 = This feature will be removed from the book.
- 1 = Some server settings will be displayed, helping the player to know what is enabled on the server.

### "ServerInfo"
Array. Allow to write multiple paragraph to share informations about the server. A guide is [available here](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/Setting-up-the-Server-Book-Tab)

### "ServerLogoPath"
String. Parameter for the logo of the server. Need to be in EDDS format and inside a mod. a url won't work.

### "RuleCategories"
Array. This where you will organize and list your rules for your server. A guide will be available later.

### "ItemRequired"
String. If kept empty (like this => "") the player will not require a specific item to open the expansion book (B). However if you add a classname inside the "" the player will require this item to open the expansion book (b).

### "ItemRequiredLocation"
Bool. 
- 0 = The player will need this item to be in his inventory. (only if ItemRequired is configured)
- 1 = The player will need this item to be in his hands.(only if ItemRequired is configured)

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/BookSettings.json