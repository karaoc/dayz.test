[![ExpansionSample-LoadingScreen](https://steamuserimages-a.akamaihd.net/ugc/1284039142817792009/810FC4F940938729C815A2051A12CE3CAD65AB53/)](https://steamcommunity.com/sharedfiles/filedetails/?id=2156696101)

Click on the picture to be redirected on our sample flag textures mod.

You will need to setup a mod with the usual **config.cpp** for a basic mod. All the files we will create will need to add new flags.

The hierarchy of the mod we have provided looks like this.

![Hierachy mod](https://i.imgur.com/lV22bA9.png)

## Config.cpp

	class CfgPatches
	{
		class **ModName**
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
		class **ModName**
		{
			dir="**ModName**";
			picture="";
			action="";
			hideName=1;
			hidePicture=1;
			name="**ModName**";
			credits="_**AuthorName**_";
			author="_**AuthorName**_";
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
						"**ModName**/Scripts/3_Game"
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
			AddFlagTexture("ModName\\data\\flag_name_co.paa", "MyFlagName"); //AddFlagTexture(Path to texture, Name)
		};
	};