Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

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

### "RuleCategorys"
Array. This where you will organize and list your rules for your server. A guide will be available later.

# Raw file

       {
        "EnableBook": 1,
        "EnableStatusTab": 1,
        "EnablePartyTab": 1,
        "EnableServerInfoTab": 1,
        "EnableServerRulesTab": 1,
        "EnableTerritoryTab": 1,
        "ShowServerSettings": 1,
        "ServerInfo": {
            "ServerButtons": [
                {
                    "IconPath": "set:expansion_iconset image:icon_group",
                    "URL": "https://exp.thurston.pw",
                    "Tooltip": "Feedback",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_discord",
                    "URL": "https://discord.io/expansion",
                    "Tooltip": "Discord",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_home",
                    "URL": "https://www.google.com",
                    "Tooltip": "Homepage",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_forums",
                    "URL": "https://www.google.com",
                    "Tooltip": "Forums",
                    "Color": -1
                },
                {
                    "IconPath": "set:expansion_iconset image:icon_patreon",
                    "URL": "https://www.patreon.com/dayzexpansion",
                    "Tooltip": "Patreon",
                    "Color": -1
                }
            ],
            "ServerSections": [
                {
                    "HasHeading": 1,
                    "HeadText": "PLACEHOLDER",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "PLACEHOLDER 2",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "PLACEHOLDER 3",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "PLACEHOLDER 4",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit amet est et sapien ullamcorper pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>"
                },
                {
                    "HasHeading": 1,
                    "HeadText": "PLACEHOLDER 5",
                    "BodyText": "<p>Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.</p>"
                }
            ],
            "ServerName": "SERVER NAME"
        },
        "ServerLogoPath": "set:expansion_gui_logos image:expansion_logo_black",
        "RuleCategorys": [
            {
                "RuleButtons": [
                    {
                        "RuleSection": {
                            "Rules": [
                                {
                                    "DetailContent": "Glichting into bases is a ban reason and will not be tolerated."
                                },
                                {
                                    "DetailContent": "Glichting under the map or clipping thrue objects will not be tolerated."
                                }
                            ],
                            "DetailLabel": "Glitching"
                        },
                        "DetailLabel": "Glitching",
                        "DetailContent": "Rule section 1 description",
                        "Icon": "DayZExpansion\\GUI\\icons\\hud\\tent_64x64.edds"
                    },
                    {
                        "RuleSection": {
                            "Rules": [
                                {
                                    "DetailContent": "Any kind of cheats or third-party programms are not allowed and will be treated accordingly."
                                }
                            ],
                            "DetailLabel": "Cheating"
                        },
                        "DetailLabel": "Cheating",
                        "DetailContent": "Rule section 2 description",
                        "Icon": "DayZExpansion\\GUI\\icons\\marker\\marker_skull.paa"
                    }
                ],
                "DisplayName": "Hacking and Cheating"
            },
            {
                "RuleButtons": [
                    {
                        "RuleSection": {
                            "Rules": [
                                {
                                    "DetailContent": "Insults of all kinds will not be tolerated unless they are part of an roleplay."
                                },
                                {
                                    "DetailContent": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut et mi non purus varius maximus. Pellentesque interdum, justo id luctus euismod, urna sapien convallis justo, non feugiat sapien orci a leo. Mauris lobortis sapien in erat interdum pretium. Integer ultrices odio lobortis lectus gravida, ac congue velit consequat. Nullam tempor lectus mollis, vulputate nibh sed, interdum ante. Donec finibus turpis purus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Aliquam non diam id odio varius dignissim. Nulla nec est ut libero imperdiet suscipit. Maecenas et arcu non purus sollicitudin venenatis."
                                }
                            ],
                            "DetailLabel": "Insults"
                        },
                        "DetailLabel": "Insults",
                        "DetailContent": "Rule section 1 description",
                        "Icon": "DayZExpansion\\GUI\\icons\\hud\\info_64x64.edds"
                    }
                ],
                "DisplayName": "Etiquette"
            }
        ],
        "RuleParagraphColor": -13330213,
        "RuleButtonColor": -13330213,
        "ShowTooltipOnRuleButton": 0
    }