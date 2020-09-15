[![ExpansionSample-LoadingScreen](https://steamuserimages-a.akamaihd.net/ugc/1284039142817792009/810FC4F940938729C815A2051A12CE3CAD65AB53/)](https://steamcommunity.com/sharedfiles/filedetails/?id=2156696101)

Click on the picture to be redirected on our sample flag textures mod.

# DISCLAIMER !

We are not going to teach you how to create a mod or convert images to .paa/.edds.

## Contents

- [config.cpp](#configcpp)

- [FlagSample.c](#flagsamplec)

- [FlagClothSample.c](#flagclothsamplec)

- [Flag dimensions](#flag-dimensions)

You will need to setup a mod with the usual **config.cpp** for a basic mod. All the files we will create will need to add new flags.

The hierarchy of the mod we have provided looks like this.

![Hierachy mod](https://i.imgur.com/lV22bA9.png)

## config.cpp
	class CfgPatches
	{
		class ExpansionFlagSample
		{
			units[] = {};
			weapons[] = {};
			requiredVersion = 0.1;
			requiredAddons[] = {"DZ_Data", "DayZExpansion_Scripts"};
		};
	};
	class CfgMods
	{
		class ExpansionFlagSample
		{
			dir = "ExpansionFlagSample";
			picture = "";
			action = "";
			hideName = 1;
			hidePicture = 1;
			name = "ExpansionFlagSample";
			credits = "Not A Banana";
			author = "Not A Banana";
			authorID = "0";
			version = "1.0";
			extra = 0;
			type = "mod";
			dependencies[] = {"Game","World","Mission"};
			class defs
			{
				class gameScriptModule
				{
					value = "";
					files[] = {"ExpansionFlagSample/scripts/3_Game"};
				};
				class worldScriptModule
				{
					value = "";
					files[] = {"ExpansionFlagSample/scripts/4_World"};
				};
			};
		};
	};

	//! Flag cloth item
	class CfgVehicles
	{
		class Flag_Base;
		class Expansion_Flag_BohemiaInteractive: Flag_Base
		{
			scope=2;
			hiddenSelectionsTextures[]=
			{
				"\ExpansionFlagSample\data\flag_bohemiainteractive_co.paa"
			};
		};
	};

## FlagSample.c
To add a flag texture you need to add the following lines and modifications to your mod within the game script module (3_Game):

	modded class ExpansionStatic
	{
		override void LoadFlagTextures()
		{
			super.LoadFlagTextures();
			// This is where you want to add or remove flags !
			AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName");
		};
	};
To add a flag you need to add the following line:

        AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName"); //AddFlagTexture(Path to texture, Name);

If you want to remove a flag that is arleady added by expansion you will need to add the following line to that modification:

	RemoveFlagTexture("DayZExpansion\\Objects\\Structures\\Flags\\data\\logos\\flag_expansion_co.paa");

This is an example for adding 2 new flags and remove the expansion logo flag from the expansion mod:

	modded class ExpansionStatic
	{
		override void LoadFlagTextures()
		{
			super.LoadFlagTextures();
			// This is where you want to add or remove flags !
			AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName");
			AddFlagTexture("ModName\\data\\flag_name2_co.paa", "MyFlagName2");
			RemoveFlagTexture("DayZExpansion\\Objects\\Structures\\Flags\\data\\logos\\flag_expansion_co.paa");
		};
	};

## FlagClothSample.c
To add the flag cloth item (#config.cpp contains the configuration) you need to add the class name of that new item to the world script module.
Simply define your item class with the correct class name like this:

	class Expansion_Flag_BohemiaInteractive extends Flag_Base {};

## Flag dimensions

The texture need to have **2:1** dimensions. For example a texture of **512 pixels** by **256 pixels** will work.