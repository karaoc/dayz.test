![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

## Description
On the server info tab of the book menu we give server owners the possibility to add hyperlink buttons and text sections to it.

Within the servers BookSettings.json you will find a section called "ServerButtons" where you are able to add buttons to the server info tab
that heads towards a special URL when clicked.


## Where do you need to go ?
Go to `DayZServer\ServerProfile (or config)\ExpansionMod\Settings` and open the `BookSettings.json`

![Expansion Server Settings Path](https://i.gyazo.com/13a0d0db7dedd48fc91ee8ba6b5024ab.png)

Inside this file you should have something similar like the following lines:
![Expansion Server Book Settings File](https://i.gyazo.com/f26040b2fa0a05267a15d36831fa819a.png)

## How does it work ?

```
	{
		"IconPath": "set:expansion_iconset image:icon_group",
		"URL": "https://exp.thurston.pw",
		"Tooltip": "Feedback",
		"Color": -1
	}
```
**REMOVE** the `,` from `},` on the last server button config entry.

#### IconPath

The string path to the image that gets used for the icon (can be a image path to a .edds or .paa file or like in the example a image set image).
Side note: Please take in note that the image have to exist on every client that should see it. If you are planing to use a image that is not in the Expansion mod or in the base game you will need to create a own mod that contains these images and every single client needs that mod loaded on there game!"

#### URL

The string URL the browser is opening after clicking the button.

#### Tooltip

A string description (should be one word) that gets displayed when ever the client is pointing on that button.

#### Color

Color integer for the icon color.


## Example

```
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
	}
],
```