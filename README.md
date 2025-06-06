## Regulated Dynamic Anomalies
Tired of DAO spawning anomalies in places that basically "softlock" you?  
This project is going to change that by blacklisting smart terrains thus not letting DAO spawn anomalies there.

This is going to be an iterative project where I request your help, so how can you help?

## How to help
1. Install the mod. (prio doesn't matter)
2. Just play as you would normally.
3. When you get to a place where you would think a DAO spawned anomaly would be annoying go to MCM -> Regulated Dynamic Anomalies and tick `Enable smart logger`

![image](https://github.com/user-attachments/assets/c1d16b42-83dc-4914-899c-94b2226b6a9c)

4. Once activated just stand where you think an anomaly spawn would softlock and press "X". This will log the map name and the smart terrain name to your log files. After this if you don't want to report more smart terrains you can go back to MCM and disable the smart logger.
5. When you close the game open `...Anomaly\appdata\logs` and open the file that is named `xray_someName.log` then press `CTRL + F` and enter this text: `[SERIOUS SMART LOGGER]` then press enter.

![image](https://github.com/user-attachments/assets/f76d3859-1e72-4431-b93b-744a080fab45)

6. You're going to see a log entry (or multiple) that looks something like this: `[SERIOUS SMART LOGGER] LevelName: l08u_brainlab, Smart name: x162_st_snork` copy these lines to a `.txt` or whatever file and post it on the mod thread.
7. You're done. Thank you for contributing!

## Maps and smarts blacklisted

```lua
--Cordon
["l01_escape"] =
{
    ["esc_smart_terrain_5_2"] = true --Anomalies blocking the entrance from Garbage
    ["esc_smart_terrain_2_12"] = true --Rookie Village
},

--Meadow
["y04_pole"] =
{
    ["pol_smart_terrain_1_1"] = true, --Anomalies spawn around the campfire in the small village, Lost Signal tasks can be blocked by them
    ["pol_sim_1"] = true --Anomalies spawn infront of the building in the factory, Lost Signal tasks can be blocked by them
},

--Garbage
["l02_garbage"] =
{
    ["gar_smart_terrain_6_3"] = true --Anomalies spawn inside the Flea Market blocking access to the area, the traders or the basement under the building
},

--Agroprom Underground
["l03u_agr_underground"] =
{
    ["agr_u_soldiers"] = true, --Anomalies can spawn blocking the entrance next to the scripted bloodsucker area
    ["agr_u_bloodsucker"] = true, --Anomalies can spawn blocking the path from the military entrance to Agro Underground
    ["agr_u_bloodsucker_2"] = true --Anomalies can spawn inside Strelok's hideout blocking the entrance
},

--Yantar
["l08_yantar"] =
{
    ["yan_smart_terrain_snork_u"] = true --Anomalies can spawn in the MM tunnels
},

--Miracle Machine (X-16)
["l08u_brainlab"] =
{
    ["x162_st_snork"] = true, --First room with snorks can be filled with anomalies
    ["x162_st_poltergeist"] = true --The entire main chamber area with platforms can spawn anomalies next to the consoles, on the platforms or on the stairs
},

--Wild Territory
["l06_rostok"] =
{
    ["ros_smart_monster5"] = true, --Anomalies can spawn in a little pathway next to the helicopter, Lost Signal tasks can be blocked by them
    ["ros_smart_killers1"] = true --Radiation patch in the sniper nest
},

--Army Warehouses
["l07_military"] =
{
    ["mil_smart_terrain_2_2"] = true, --Radiation patch on entry to Army Warehouses from Dead City
    ["mil_smart_terrain_4_8"] = true --Radiation patch and possibly other anomalies around Gatekeeper spot (i doubt it's an actual issue but i guess it could happen..)
},

--Dead City
["l09_deadcity"] =
{
    ["cit_killers_vs_bandits"] = true --Radiation along with gravitational anomalies in the building in the middle of the map
},

--Brain Scorcher (X-19)
["l10u_bunker"] =
{
    ["bun2_tushkano_lair"] = true, --Anomalies blocking route to the main switch
    ["bun_krovosos_nest"] = true,
    ["bun2_st_bloodsucker"] = true
},

--Limansk
["l10_limansk"] =
{
    ["lim_smart_terrain_4"] = true --Anomalies blocking a pathway through the city (linear design is pain)
},

--Pripyat
["l11_pripyat"] =
{
    ["pri_smart_bloodsucker_lair1"] = true, --Anomalies blocking the entrance from Jupiter
    ["pri_smart_pseudodog_lair1"] = true --Anomalies blocking the entrance from Outskirts
},

--Outskirts
["pripyat"] =
{
    ["pri_a28_heli"] = true --Anomalies spawning next to the Prometheus Theater, can block Operation Afterglow and the Living Fire quest
},

--Red Forest
["l10_red_forest"] =
{
    ["red_smart_terrain_monsters_2"] = true, --The cave that you have to go through to get to the south eastern part of Red Forest
    ["red_smart_terrain_3_2"] = true --SIN base
}
```
