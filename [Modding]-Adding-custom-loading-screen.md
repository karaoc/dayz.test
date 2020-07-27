[![ExpansionSample-LoadingScreen](https://steamuserimages-a.akamaihd.net/ugc/1284039142817792009/810FC4F940938729C815A2051A12CE3CAD65AB53/)](https://steamcommunity.com/sharedfiles/filedetails/?id=2156698657)

Click on the picture to be redirected on our sample flag textures mod.

# DISCLAIMER !

We are not going to teach you how to create a mod or convert to paa. Youtube already have enough tutorials for this !

## Contents

- [Config.cpp](#configcpp)

- [LoadingScreens.c](#loadingscreensc)

- [Converting your image to edds](#converting-your-image-to-edds)

You will need to setup a mod with the usual **config.cpp** for a basic mod. All the files we will create will need to add new flags.

The hierarchy of the mod we have provided looks like this.

![Hierachy mod](https://i.imgur.com/zMt9kAX.png)

## Config.cpp

	class CfgPatches
	{
		class MyModName
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
		class MyModName
		{
			dir="MyModName";
			picture="";
			action="";
			hideName=1;
			hidePicture=1;
			name="MyModName";
			credits="MyName";
			author="MyName";
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
						"MyModName/Scripts/3_Game"
					};
				};
				class worldScriptModule
				{
					value="";
					files[]=
					{
						"MyModName/Scripts/4_World"
					};
				};
				class missionScriptModule
				{
					value="";
					files[]=
					{
						"MyModName/Scripts/5_Mission"
					};
				};
			};
		};
	};

## LoadingScreens.c

	const string LOADING_SCREENS_PATH = "ExpansionLoadingScreenSample/data/CustomLoading"; // Change this to the path of your edds files + file names sans the number. Loading Screens must be named "CustomLoading1.edds", "CustomLoading2.edds", etc 
	//Use Workbench to convert .tga files to .edds. Simply add the .tga files to the dir you wish, right click, and "Register Resource and import" 
	const int LOADING_SCREENS_COUNT = 2; // The Amount of loading screens you are adding
	modded class LoadingScreen 
	{
		override void Show()
		{
			//m_Backgrounds.Clear(); //If you want to use *only* your screens, uncomment this. If you want to simply add to the existing loading screens, you can keep this commented. 
			for (int i = 0; i < LOADING_SCREENS_COUNT; i++) {
				m_Backgrounds.Insert(new ExpansionLoadingScreenBackground(LOADING_SCREENS_PATH + (i + 1) + ".edds"));
			}
			super.Show();
		}
	}
	modded class LoginQueueBase 
	{
		override Widget Init()
		{
			super.Init();
			//m_Backgrounds.Clear(); //If you want to use *only* your screens, uncomment this. If you want to simply add to the existing loading screens, you can keep this commented. 
			for (int i = 0; i < LOADING_SCREENS_COUNT; i++) {
				m_Backgrounds.Insert(new ExpansionLoadingScreenBackground(LOADING_SCREENS_PATH + (i + 1) + ".edds"));
			}
			return super.Init();
		}
	}
	modded class LoginTimeBase 
	{
		override Widget Init()
		{
			super.Init();
			//m_Backgrounds.Clear(); //If you want to use *only* your screens, uncomment this. If you want to simply add to the existing loading screens, you can keep this commented. 
			for (int i = 0; i < LOADING_SCREENS_COUNT; i++) {
				m_Backgrounds.Insert(new ExpansionLoadingScreenBackground(LOADING_SCREENS_PATH + (i + 1) + ".edds"));
			}
			return super.Init();
		}
	}

## Converting your image to edds
