[![ExpansionSample-LoadingScreen](https://steamuserimages-a.akamaihd.net/ugc/1284039142817792009/810FC4F940938729C815A2051A12CE3CAD65AB53/)](https://steamcommunity.com/sharedfiles/filedetails/?id=2156696101)

Click on the picture to be redirected on our sample flag textures mod.

# DISCLAIMER !

We are not going to teach you how to create a mod or convert to paa. Youtube already have enough tutorials for this !

## Contents

- [Config.cpp](#configcpp)

- [FlagSample.c](#flagsamplec)

- [Flag dimensions](#flag-dimensions)

You will need to setup a mod with the usual **config.cpp** for a basic mod. All the files we will create will need to add new flags.

The hierarchy of the mod we have provided looks like this.

![Hierachy mod](https://i.imgur.com/lV22bA9.png)

## Config.cpp

	class CfgPatches
	{
		class ModName
		{
			units[]={};
			weapons[]={};
			requiredVersion=0.1;
			requiredAddons[]=
			{
				"DayZExpansion_Scripts"
			};
		};
	};
	class CfgMods
	{
		class ModName
		{
			dir="ModName";
			picture="";
			action="";
			hideName=1;
			hidePicture=1;
			name="ModName";
			credits="AuthorName";
			author="AuthorName";
			authorID="0";
			version="1.0";
			extra=0;
			type="mod";
			dependencies[]=
			{
				"Game",
				"World",
				"Mission"
			};
			class defs
			{
				class gameScriptModule
				{
					value="";
					files[]=
					{
						"ModName/Scripts/3_Game"
					};
				};
			};
		};
	};

## FlagSample.c

	modded class ExpansionStatic
	{
		override void LoadFlagTextures()
		{
			super.LoadFlagTextures();
			// This is where you want to add or remove flags !
		};
	};

To add a flag you need to add the following line

	AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName"); //AddFlagTexture(Path to texture, Name)

It should look like this

	modded class ExpansionStatic
	{
		override void LoadFlagTextures()
		{
			super.LoadFlagTextures();
			// This is where you want to add or remove flags !
			AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName");
		};
	};

If you want to add another flag, add another "AddFlagTexture" like you just did.

	AddFlagTexture("ModName\\data\\flag_name2_co.paa", "MyFlagName2"); //AddFlagTexture(Path to texture, Name)

If you want to remove a flag already ingame you will need to add the following line :

	RemoveFlagTexture("DayZExpansion\\Objects\\Structures\\Flags\\data\\logos\\flag_expansion_co.paa"); //If you have a flag you want removed, simply run this with the path to the texture as the argument. 

In this example, we are now removing the expansion flag :

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

## Flag dimensions

The texture need to have **2:1** dimensions. For example a texture of **256 pixels** by **128 pixels** will work.

![dimenssions](https://i.imgur.com/hKIQy5j.jpg)