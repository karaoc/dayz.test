![DayZ Expansion Book Menu](https://i.gyazo.com/95b6767f86330d991789c66d47161156.jpg)

## Where do you need to go ?

Go to `DayZServer\ServerProfile (or config)\ExpansionMod\Settings` and open the `BookSettings.json`

![Expansion Server Settings Path](https://i.imgur.com/yKiftOu.png)

Inside this file you should have something similar like the following lines:

![Expansion Server Book Settings File](https://i.imgur.com/y1e69gP.png)

## How does it work ?

```
{
    "HasHeading": 1,
    "HeadText": "My First title !",
    "BodyText": "<p>This is a paragraph, some HTML stuff can be used based on what the game allow us to use.</p>"
},
{
    "HasHeading": 1,
    "HeadText": "My Second title :)",
    "BodyText": "<p>You can also use <br/> to go on the next line ! </p>"
},
{
    "HasHeading": 0,
    "HeadText": "This text won't be displayed in the book because the line above is set to 0",
    "BodyText": "<p>But I'm still visible !</p>"
}
```
**REMOVE** the `,` from `},` on the last server button config entry.

#### HasHeading

This is a "boolean" (yes/no aka on/off). This is used to hide or show the title (HeadText) bellow it.

- 0 = OFF (doesn't show the title)
- 1 = ON (the title will be visible)

#### HeadText

The string URL the browser is opening after clicking the button.

#### BodyText

A string description (should be one word) that gets displayed when ever the client is pointing on that button.

## Example

```
"ServerSections": [
    {
        "HasHeading": 1,
        "HeadText": "Hero Trader",
        "BodyText": "<p>The Hero Trader is a very nice guy living in a old store near Kamenka. Sadly his Helicopter got shutdown by some bandits !</p>"
    },
    {
        "HasHeading": 1,
        "HeadText": "Bandit Trader",
        "BodyText": "<p>Rumors says they have settle at Balota.<br/>However nobody cameback...</p>"
    },
    {
        "HasHeading": 1,
        "HeadText": "Crafting guide",
        "BodyText": "<p>1 rope + 3 sticks = TerritoryKit<br>1 rope + 2 sticks = FenceKit<br>1 rope + 4 sticks = Watchtowerkit</p>"
    }
],
"ServerName": "The tale of the Banditz"
```