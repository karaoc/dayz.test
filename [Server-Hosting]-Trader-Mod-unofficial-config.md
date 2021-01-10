![DayZ Expansion](https://i.imgur.com/cTbqjAr.png)

# WARNING !

This config is not up to date and **is NOT official**. If anyone among the community want to share their own trader config we have no issues sharing it there. Same for trader mapping.


## Adding a Aircraft Trader to Chernarus:

### 1. Make sure you have the following trader mod installed: https://steamcommunity.com/sharedfiles/filedetails/?id=1590841260
### 2. Follow the install instructions on that page
### 3. Add the following inside of your *TraderObjects.txt*
```
// North West Aircraft:

<TraderMarker> 			6
<TraderMarkerPosition>	4080,    339,    10801
<TraderMarkerSafezone>	30
<VehicleSpawn>			4092,	340,	10782		// Vehicle Spawnpoint for Trader; 	Coordinate X, 	Coordinate Y, 	Coordinate Z (optional)
<VehicleSpawnOri>		-90,		0,			0			// Vehicle Spawnpoint Orientation; 	Yaw, 			Pitch, 			Roll	 	 (optional)
```

and make sure this is under your *// Kumyrna:* config around line 59 (Using Notepad++

### 4. Add the following also inside of your *TraderObjects.txt*
```
// North West Aircraft:
<Object> 			SurvivorM_Taiki
<ObjectPosition>	4080,    339,    10801
<ObjectOrientation>	90,	0,			0
<ObjectAttachment>	AviatorGlasses
<ObjectAttachment>	BomberJacket_Black
<ObjectAttachment>	Jeans_Black
<ObjectAttachment>	CombatBoots_Black


<Object>			Land_Mil_Fortified_Nest_Small
<ObjectPosition>	4079.080811, 340.034180, 10801.098633
<ObjectOrientation>	80.999992,	0,			0
 
<Object>			Land_Mil_CamoNet_Roof_east
<ObjectPosition>	4079.046143, 340.272644, 10800.850586
<ObjectOrientation>	-98.000015,			0,			0
 
<Object>			Wreck_UH1Y
<ObjectPosition>	4074.843750, 340.806946,  10812.857422
<ObjectOrientation>	-104.000000,0,			0
 
<Object>			Wreck_Mi8
<ObjectPosition>	4073.852783, 340.647949, 10791.951172
<ObjectOrientation>	-45.000000,0,			0
 
<Object>			Land_Misc_Well_Pump_Yellow
<ObjectPosition>	4070.367432, 339.726288, 10800.843750
<ObjectOrientation>	0,	0,			0
 
 <Object>			Land_FuelStation_Feed
<ObjectPosition>	4087.541016, 340.008636, 10779.255859
<ObjectOrientation>	63,	0,			0
```
Make sure this is at the bottom of the file just above *//<OpenFile> FileName.txt*

### 5. Add the following to your *TraderConfig.txt*
```
<Trader> Aircraft Trader
	<Category> Helicopters
	ExpansionUh1h, V, 150000, 75000
	ExpansionMh6, V, 150000, 75000
	ExpansionMerlin, v, 150000, 75000
	ExpansionGyrocopter, V, 35000, 17500
	
	<Category> Helicopter Parts
	ExpansionHelicopterBattery, *, 4000, 2000
	CarRadiator, *, 500, 250
	SparkPlug, *, 250, 125
	HeadlightH7, *, 75, 30
	ExpansionHydraulicHoses, *, 300, 150
	ExpansionIgniterPlug, *, 500, 250
```
Make sure this placed towards the bottom just above the *<Category> Keys* section at around line 1184

Adjust pricing as you wish. 

### 6. Add the map marker to your map by editing your MapSettings.json in your ExpansionMod
```
{
    "m_UID": "NWAircraftTrader",
    "m_Visibility": 6,
    "m_Is3D": 1,
    "m_Text": "Aircraft Trader",
    "m_IconName": "Helicopter",
    "m_Color": -13710223,
    "m_Position": [
		4080,    
		339,    
		10801
           ]
        }
    ]
```
For help adding markers see the documentation here: https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-server-markers

## Trader Vehicle Parts

    <VehicleParts> ExpansionUh1h
    ExpansionHelicopterBattery
    ExpansionHydraulicHoses
    CarRadiator
    ExpansionIgniterPlug

    <VehicleParts> ExpansionGyrocopter
    ExpansionHelicopterBattery
    CarRadiator
    SparkPlug
    HeadlightH7

    <VehicleParts> ExpansionMh6
    ExpansionHelicopterBattery
    CarRadiator
    ExpansionIgniterPlug
    ExpansionHydraulicHoses
    HeadlightH7
    Expansion_Mh6_Door_1_1
    Expansion_Mh6_Door_1_2
    Expansion_Mh6_Door_2_1
    Expansion_Mh6_Door_2_2

    <VehicleParts> ExpansionMerlin
    ExpansionHelicopterBattery
    CarRadiator
    ExpansionHydraulicHoses
    ExpansionIgniterPlug
    HeadlightH7
    HeadlightH7
    ExpansionMerlinFrontWheel
    ExpansionMerlinFrontWheel
    ExpansionMerlinBackWheel
    ExpansionMerlinBackWheel
