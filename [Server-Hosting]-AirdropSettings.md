Last updated the 18th of September 2020 - [Return to the summary](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Server-settings/)

**WARNING** - The AirdropSettings only affect personnal airdrops and NOT mission airdrops from the mission file. Even if they seems to be the same they are not overriding the airdrop missions. If you want to customize airdrop mission please follow [this guide](https://github.com/salutesh/DayZ-Expansion-Scripts/wiki/%5BServer-Hosting%5D-Adding-custom-airdrops)


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


    {
        "ServerMarkerOnDropLocation": 1,
        "Server3DMarkerOnDropLocation": 1,
        "ShowAirdropTypeOnMarker": 0,
        "Height": 750,
        "Speed": 1500,
        "ItemCount": 50,
        "Containers": [
            {
                "Container": "ExpansionAirdropContainer",
                "Loot": [
                    {
                        "Name": "AKS74U",
                        "Attachments": [
                            "AKS74U_Bttstck"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK_WoodBttstck",
                            "AK_WoodHndgrd"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "SKS",
                        "Attachments": [
                            "PUScopeOptic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SKS",
                        "Attachments": [
                            "SKS_Bayonet"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SKS",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "UMP45",
                        "Attachments": [
                            "UniversalLight"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "UMP45",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Mosin9130",
                        "Attachments": [
                            "PUScopeOptic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mosin9130",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "B95",
                        "Attachments": [
                            "HuntingOptic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "B95",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "CZ527",
                        "Attachments": [
                            "HuntingOptic"
                        ],
                        "Chance": 0.3
                    },
                    {
                        "Name": "CZ527",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "CZ75",
                        "Attachments": [
                            "TLRLight"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "CZ75",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "FNX45",
                        "Attachments": [
                            "TLRLight"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "FNX45",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Expansion_Kedr",
                        "Attachments": [
                            "PistolSuppressor"
                        ],
                        "Chance": 0.2
                    },
                    {
                        "Name": "Expansion_Kedr",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Mp133Shotgun",
                        "Attachments": [],
                        "Chance": 0.8
                    },
                    {
                        "Name": "Winchester70",
                        "Attachments": [
                            "HuntingOptic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Winchester70",
                        "Attachments": [],
                        "Chance": 0.4
                    },
                    {
                        "Name": "Expansion_DT11",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Binoculars",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "ChernarusMap",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Rangefinder",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "ExpansionGPS",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "BoxCerealCrunchin",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "PeachesCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "BakedBeansCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SpaghettiCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SardinesCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "TunaCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "WaterBottle",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "CanOpener",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "KitchenKnife",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "BallisticHelmet_UN",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "DirtBikeHelmet_Chernarus",
                        "Attachments": [
                            "DirtBikeHelmet_Visor"
                        ],
                        "Chance": 0.3
                    },
                    {
                        "Name": "SewingKit",
                        "Attachments": [],
                        "Chance": 0.25
                    },
                    {
                        "Name": "LeatherSewingKit",
                        "Attachments": [],
                        "Chance": 0.25
                    },
                    {
                        "Name": "WeaponCleaningKit",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Lockpick",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "GhillieAtt_Mossy",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Mag_Expansion_Kedr_20Rnd",
                        "Attachments": [],
                        "Chance": 0.8
                    },
                    {
                        "Name": "Mag_CZ527_5rnd",
                        "Attachments": [],
                        "Chance": 0.9
                    },
                    {
                        "Name": "Mag_CZ75_15Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Mag_FNX45_15Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Mag_UMP_25Rnd",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "AmmoBox_9x39_20Rnd",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "AmmoBox_9x19_25Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_762x39Tracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "AmmoBox_762x39_20Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_45ACP_25Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_308WinTracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "AmmoBox_308Win_20Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_12gaSlug_10Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_12gaRubberSlug_10Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "AmmoBox_12gaPellets_10Rnd",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_9x39",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "Ammo_762x39Tracer",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "Ammo_762x39",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_45ACP",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_308WinTracer",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "Ammo_308Win",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_12gaSlug",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_12gaRubberSlug",
                        "Attachments": [],
                        "Chance": 1
                    },
                    {
                        "Name": "Ammo_12gaPellets",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing"
                        ],
                        "Chance": 0.03
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "SalineBagIV"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "CharcoalTablets",
                            "Morphine"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "Epinephrine",
                            "StartKitIV"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "Morphine",
                            "SalineBagIV"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "PainkillerTablets",
                            "Epinephrine"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "TetracyclineAntiBiotics",
                            "Morphine"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "VitaminBottle"
                        ],
                        "Chance": 0.05
                    }
                ]
            },
            {
                "Container": "ExpansionAirdropContainer_Medical",
                "Loot": [
                    {
                        "Name": "BandageDressing",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Morphine",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Epinephrine",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "TacticalBaconCan",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "PainkillerTablets",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "CharcoalTablets",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "TetracyclineAntiBiotics",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "DisinfectantSpray",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "DisinfectantAlcohol",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "VitaminBottle",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "StartKitIV",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "SalineBagIV",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SalineBag",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "BloodBagEmpty",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "BloodBagIV",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "BloodTestKit",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "BloodTestKit",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "MedicalScrubsHat_Blue",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsHat_White",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsHat_Green",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsPants_Blue",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsPants_White",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsPants_Green",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsShirt_Blue",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsShirt_White",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "MedicalScrubsShirt_Green",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "NioshFaceMask",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "SurgicalGloves_Blue",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "SurgicalGloves_LightBlue",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "SurgicalGloves_Green",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "BandageDressing"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing",
                            "BandageDressing"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "Morphine",
                            "BandageDressing"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "SalineBagIV"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "PainkillerTablets",
                            "DisinfectantAlcohol"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "CharcoalTablets",
                            "Morphine"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "Epinephrine",
                            "StartKitIV"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "TetracyclineAntiBiotics",
                            "VitaminBottle"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "Morphine",
                            "SalineBagIV"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "PainkillerTablets",
                            "Epinephrine"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "TetracyclineAntiBiotics",
                            "Morphine"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "VitaminBottle",
                            "SurgicalGloves_Blue"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "BandageDressing",
                            "VitaminBottle"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FirstAidKit",
                        "Attachments": [
                            "CharcoalTablets",
                            "DisinfectantAlcohol"
                        ],
                        "Chance": 0.18
                    }
                ]
            },
            {
                "Container": "ExpansionAirdropContainer_Basebuilding",
                "Loot": [
                    {
                        "Name": "NailBox",
                        "Attachments": [],
                        "Chance": 0.8
                    },
                    {
                        "Name": "DuctTape",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "MetalPlate",
                        "Attachments": [],
                        "Chance": 0.25
                    },
                    {
                        "Name": "WoodenPlank",
                        "Attachments": [],
                        "Chance": 0.5
                    },
                    {
                        "Name": "Hammer",
                        "Attachments": [],
                        "Chance": 0.4
                    },
                    {
                        "Name": "Shovel",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Pliers",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "WoodAxe",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Crowbar",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Hacksaw",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Handsaw",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SledgeHammer",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Hatchet",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionCodeLock",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "BarbedWire",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "MetalWire",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionHescoKit",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "ExpansionBarbedWireKit",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "ExpansionCamoBoxKit",
                        "Attachments": [],
                        "Chance": 0.18
                    },
                    {
                        "Name": "ExpansionGunrack",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "ExpansionCone",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionSignDanger",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionSignDanger2",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionSignDanger3",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionSignRoadBarrier",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "ExpansionSafeMini",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "ExpansionSafeMedium",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "ExpansionSafeLarge",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "ExpansionCamoTentKit",
                        "Attachments": [],
                        "Chance": 0.25
                    },
                    {
                        "Name": "MediumTent",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "LargeTent",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "CarTent",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "CamoNet",
                        "Attachments": [],
                        "Chance": 0.3
                    }
                ]
            },
            {
                "Container": "ExpansionAirdropContainer_Military",
                "Loot": [
                    {
                        "Name": "AK101",
                        "Attachments": [
                            "AK_PlasticBttstck",
                            "AK_PlasticHndgrd"
                        ],
                        "Chance": 0.12
                    },
                    {
                        "Name": "AK74",
                        "Attachments": [
                            "AK74_WoodBttstck",
                            "AK74_Hndgrd"
                        ],
                        "Chance": 0.135
                    },
                    {
                        "Name": "AK74",
                        "Attachments": [
                            "AK_FoldingBttstck",
                            "AK74_Hndgrd"
                        ],
                        "Chance": 0.115
                    },
                    {
                        "Name": "AK74",
                        "Attachments": [
                            "AK_FoldingBttstck",
                            "AK74_Hndgrd",
                            "AK_Bayonet"
                        ],
                        "Chance": 0.125
                    },
                    {
                        "Name": "AK74",
                        "Attachments": [
                            "KobraOptic",
                            "AK_WoodHndgrd",
                            "AK74_WoodBttstck"
                        ],
                        "Chance": 0.12
                    },
                    {
                        "Name": "AKS74U",
                        "Attachments": [
                            "AK74_WoodBttstck"
                        ],
                        "Chance": 0.25
                    },
                    {
                        "Name": "AKS74U",
                        "Attachments": [
                            "AKS74U_Bttstck"
                        ],
                        "Chance": 0.3
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK_FoldingBttstck",
                            "AK_RailHndgrd"
                        ],
                        "Chance": 0.25
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK_WoodBttstck",
                            "AK_WoodHndgrd",
                            "KobraOptic"
                        ],
                        "Chance": 0.26
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK_PlasticBttstck",
                            "AK_RailHndgrd"
                        ],
                        "Chance": 0.26
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK74_WoodBttstck",
                            "AK74_Hndgrd"
                        ],
                        "Chance": 0.27
                    },
                    {
                        "Name": "AKM",
                        "Attachments": [
                            "AK_PlasticBttstck",
                            "AK_RailHndgrd",
                            "UniversalLight"
                        ],
                        "Chance": 0.26
                    },
                    {
                        "Name": "Expansion_M16",
                        "Attachments": [
                            "ACOGOptic"
                        ],
                        "Chance": 0.14
                    },
                    {
                        "Name": "Expansion_M16",
                        "Attachments": [
                            "UniversalLight"
                        ],
                        "Chance": 0.13
                    },
                    {
                        "Name": "Expansion_M16",
                        "Attachments": [],
                        "Chance": 0.18
                    },
                    {
                        "Name": "M4A1",
                        "Attachments": [
                            "M4_CarryHandleOptic",
                            "M4_OEBttstck",
                            "M4_PlasticHndgrd"
                        ],
                        "Chance": 0.14
                    },
                    {
                        "Name": "M4A1",
                        "Attachments": [
                            "BUISOptic",
                            "M4_CQBBttstck",
                            "M4_RisHndgrd"
                        ],
                        "Chance": 0.13
                    },
                    {
                        "Name": "M4A1",
                        "Attachments": [
                            "ACOGOptic",
                            "M4_MPBttstck",
                            "M4_MPHndgrd"
                        ],
                        "Chance": 0.14
                    },
                    {
                        "Name": "M4A1",
                        "Attachments": [
                            "BUISOptic",
                            "M4_CQBBttstck",
                            "M4_RisHndgrd",
                            "UniversalLight"
                        ],
                        "Chance": 0.18
                    },
                    {
                        "Name": "FAL",
                        "Attachments": [
                            "Fal_OeBttstck"
                        ],
                        "Chance": 0.12
                    },
                    {
                        "Name": "FAL",
                        "Attachments": [
                            "Fal_FoldingBttstck"
                        ],
                        "Chance": 0.12
                    },
                    {
                        "Name": "SVD",
                        "Attachments": [
                            "PSO1Optic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "SVD",
                        "Attachments": [],
                        "Chance": 0.18
                    },
                    {
                        "Name": "Saiga",
                        "Attachments": [
                            "Saiga_Bttstck",
                            "KobraOptic"
                        ],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Saiga",
                        "Attachments": [
                            "Saiga_Bttstck"
                        ],
                        "Chance": 0.12
                    },
                    {
                        "Name": "Expansion_M79",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "ExpansionRPG7",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "ExpansionLAW",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "AK_RailHndgrd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "AK_Bayonet",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "KobraOptic",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "UniversalLight",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "KobraOptic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "UniversalLight",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "ACOGOptic",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "M4_RisHndgrd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M9A1_Bayonet",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mosin_Bayonet",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PUScopeOptic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "TLRLight",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "TLRLight",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "SKS_Bayonet",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M68Optic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M4_T3NRDSOptic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "FNP45_MRDSOptic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "ExpansionReflexMRSOptic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PSO1Optic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PSO11Optic",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M68Optic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "M4_T3NRDSOptic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "ExpansionReflexMRSOptic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "PSO1Optic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "PSO11Optic",
                        "Attachments": [
                            "Battery9V"
                        ],
                        "Chance": 0.08
                    },
                    {
                        "Name": "RGD5Grenade",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "M67Grenade",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "M18SmokeGrenade_Red",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M18SmokeGrenade_Green",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M18SmokeGrenade_Yellow",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M18SmokeGrenade_Purple",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "M18SmokeGrenade_White",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "RDG2SmokeGrenade_Black",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "RDG2SmokeGrenade_White",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "LandMineTrap",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_AK101_30Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_AK74_30Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_AKM_30Rnd",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "Mag_AKM_Drum75Rnd",
                        "Attachments": [],
                        "Chance": 0.06
                    },
                    {
                        "Name": "Mag_AKM_Palm30Rnd",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Mag_CMAG_20Rnd",
                        "Attachments": [],
                        "Chance": 0.3
                    },
                    {
                        "Name": "Mag_CMAG_30Rnd",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Mag_CMAG_40Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_FAL_20Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_STANAGCoupled_30Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Mag_STANAG_30Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_SVD_10Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Mag_Saiga_5Rnd",
                        "Attachments": [],
                        "Chance": 0.15
                    },
                    {
                        "Name": "Mag_Saiga_8Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Mag_Saiga_Drum20Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "AmmoBox_762x54Tracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "AmmoBox_762x54_20Rnd",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "AmmoBox_762x39Tracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.06
                    },
                    {
                        "Name": "AmmoBox_762x39_20Rnd",
                        "Attachments": [],
                        "Chance": 0.09
                    },
                    {
                        "Name": "AmmoBox_556x45Tracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "AmmoBox_556x45_20Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "AmmoBox_545x39Tracer_20Rnd",
                        "Attachments": [],
                        "Chance": 0.06
                    },
                    {
                        "Name": "AmmoBox_545x39_20Rnd",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_762x54Tracer",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_762x54",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Ammo_762x39Tracer",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Ammo_762x39",
                        "Attachments": [],
                        "Chance": 0.12
                    },
                    {
                        "Name": "Ammo_556x45Tracer",
                        "Attachments": [],
                        "Chance": 0.07
                    },
                    {
                        "Name": "Ammo_556x45",
                        "Attachments": [],
                        "Chance": 0.11
                    },
                    {
                        "Name": "Ammo_545x39Tracer",
                        "Attachments": [],
                        "Chance": 0.07
                    },
                    {
                        "Name": "Ammo_545x39",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_White",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_Red",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_Green",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_Yellow",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_Purple",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Smoke_Teargas",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_White",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_Red",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_Green",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_Yellow",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_Purple",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "Ammo_Expansion_M203_Sticky_Smoke_Teargas",
                        "Attachments": [],
                        "Chance": 0.02
                    },
                    {
                        "Name": "Ammo_Expansion_M203_HE",
                        "Attachments": [],
                        "Chance": 0.7
                    },
                    {
                        "Name": "ExpansionAmmoRPG",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "UKAssVest_Black",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "UKAssVest_Camo",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "UKAssVest_Khaki",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "UKAssVest_Olive",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "HighCapacityVest_Black",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "HighCapacityVest_Olive",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PlateCarrierVest",
                        "Attachments": [],
                        "Chance": 0.08
                    },
                    {
                        "Name": "PlateCarrierHolster",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PlateCarrierPouches",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "PlateCarrierVest",
                        "Attachments": [
                            "PlateCarrierHolster",
                            "PlateCarrierPouches"
                        ],
                        "Chance": 0.05
                    },
                    {
                        "Name": "TacticalBaconCan",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "Bear_Pink",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "GhillieAtt_Mossy",
                        "Attachments": [],
                        "Chance": 0.2
                    },
                    {
                        "Name": "GhillieHood_Mossy",
                        "Attachments": [],
                        "Chance": 0.1
                    },
                    {
                        "Name": "GhillieBushrag_Mossy",
                        "Attachments": [],
                        "Chance": 0.05
                    },
                    {
                        "Name": "GhillieSuit_Mossy",
                        "Attachments": [],
                        "Chance": 0.05
                    }
                ]
            }
        ]
    }