Last updated the 19th of November 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

***

### "VehicleSync" - **CURRENTLY DOESNT WORK**
Integrer.
- 0 = Vehicles will be simulated by the Server and only the server.
- 1 = Vehicles will be simulated by the Server prediciting player actions. To make it easy to understand, it's Client and server sync. 
- 2 = Vehicles will be simulated by the client (player).

### "VehicleRequireKeyToStart"
Bool.
- 0 = Even if your car is paired to a key, you don't need to have the key in the vehicle inventory or on yourself.
- 1 = You will need a car key paired to the vehicle to start the engine.

### "VehicleRequireAllDoors"
Bool.
- 0 = Even if you are missing some doors, you can still lock the vehicle.
- 1 = You will need all the doors of the car to lock your vehicle.

### "VehicleLockedAllowInventoryAccess"
Bool.
- 0 = Players will need to unlock the vehicle to access the inventory.
- 1 = Allow players to access the inventory of the vehicle even if this vehicle is locked.

### "VehicleLockedAllowInventoryAccessWithoutDoors"
Bool.
- 0 = Even if some doors are missing, players won't be able to access the inventory of this locked vehicle.
- 1 = Allow players to access inventory of the vehicle only if this vehicle is missing one or multiple doors.

### "EnableWindAerodynamics"
Bool.
- 0 = The helicopters won't have wind simulation.
- 1 = Enable wind simulation for helicopters.

### "EnableTailRotorDamage"
Bool.
- 0 = rotors of helicopters can't be damaged.
- 1 = rotors of helicopters can be damaged and will spin if destroy making the helicopters almost unusable.

### "PlayerAttachment"
Bool.
- 0 = Players will fall and take damage like in vanilla.
- 1 = Allow players to stay on moving objects like cars, helicopters, planes or boats.

### "Towing"
Bool.
- 0 = Towing is disabled.
- 1 = Allow cars to tow other cars. Helicopters can tow any types vehicles.

### "EnableHelicopterExplosions"
Bool.
- 0 = Helicopters won't explode.
- 1 = Helicopters can explode.

# Raw file

https://github.com/ExpansionModTeam/DayZ-Expansion-Settings/blob/master/VehicleSettings.json