![DayZ Expansion Book Menu](https://i.gyazo.com/95b6767f86330d991789c66d47161156.jpg)

## Where do you need to go ?

Go to `DayZServer\ServerProfile (or config)\ExpansionMod\Settings` and open the `BookSettings.json`

![Expansion Server Settings Path](https://i.imgur.com/yKiftOu.png)

Inside this file you should have something similar like the following lines:
![Expansion Server Book Settings File](https://i.gyazo.com/f26040b2fa0a05267a15d36831fa819a.png)

## How does it work ?

```
{
    "IconPath": "set:expansion_iconset image:icon_discord",
    "URL": "https://discord.com",
    "Tooltip": "Discord",
    "Color": -1
},
{
    "IconPath": "set:expansion_iconset image:icon_twitter",
    "URL": "https://twitter.com",
    "Tooltip": "Twitter",
    "Color": -1
}
```
**REMOVE** the `,` from `},` on the last server button config entry.

#### IconPath

The string path to the image that gets used for the icon (can be a image path to a .edds or .paa file or like in the example a image set image).

Side note: Please take in note that the image have to exist on every client that should see it. If you are planing to use a image that is not in the Expansion mod or in the base game you will need to create a own mod that contains these images and every single client needs that mod loaded on there game!

_set:expansion_iconset image:ICON_NAME_HERE_

The icons you can use by default are the following :

    icon_search
    icon_namelabel
    icon_marker
    icon_removemarker
    icon_edit
    icon_cancel
    icon_plus
    icon_minus
    icon_blood
    icon_gender
    icon_bloodbag
    icon_weight
    icon_right
    icon_left
    icon_health
    icon_bloodtype
    icon_expansion_white
    icon_options
    icon_territory
    icon_patreon
    icon_position
    icon_discord
    icon_reddit
    icon_steam
    icon_github
    icon_home
    icon_forums
    icon_twitter
    icon_youtube
    icon_settings
    icon_exit
    icon_close
    icon_group
    icon_profile
    icon_status
    icon_map
    icon_info
    icon_events
    arrow_left
    arrow_right
    map
    compass
    mountains
    arrow_up
    arrow_down
    clock_blank
    clock_filled
    water_border
    water_low
    water_full
    water_normal
    water_high

#### URL

The string URL the browser is opening after clicking the button.

#### Tooltip

A string description (should be one word) that gets displayed when ever the client is pointing on that button.

#### Color

The color of the icon, use this [this website to generate the color](https://thurston.pw/public/color.php) you want to apply on your marker !

**Warning** Values you have to enter have to be between 1 and 255. 0 is not a valid option !

You can also this value to **-1** to keep it as default


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
        "URL": "https://www.google.com",
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
```