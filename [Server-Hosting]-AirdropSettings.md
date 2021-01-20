Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

**WARNING** - The AirdropSettings only affect **personnal airdrops** and NOT mission airdrops from the mission file. Even if they seems to be the same they are not overriding the airdrop missions. If you want to customize airdrop mission please follow [this guide](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-custom-airdrops)

***

### "ServerMarkerOnDropLocation"
Bool.
- 0 = No marker will be created to show the exact location of the airdrop drop point.
- 1 = The server will create a marker on the map on the airdrop drop location (where the crate will land).

### "Server3DMarkerOnDropLocation"
Bool. If "ServerMarkerOnDropLocation" is set to 0 you can ignore this setting.
- 0 = The marker will not be displayed in 3D.
- 1 = The marker will be also in 3D.

### "ShowAirdropTypeOnMarker"
Bool. If "ServerMarkerOnDropLocation" is set to 0 you can ignore this setting.
- 0 = The marker name will not have the airdrop type in his name.
- 1 = The marker name will specify what type of airdrop it is (Military, Medical, Basebuilding for example).

### "Height"
Float. The altitude the plane will fly at.

### "Speed"
Float. The speed of the plane. This will not change the speed of the crate falling.

### "ItemCount"
The amount of items the dropped crate will have.

### "Containers"
What loot could spawn inside this classname.
- Name: You have to give the exact Classname of the item
- Attachments: his attachements if you want it to spawn with items attached to it.
- Chance: The chance of spawning (1.00 = 100% and 0.00 = 0%)

Please make sure the last } of the loot list doesn't have the , in }, like in the example !

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/AirdropSettings.json