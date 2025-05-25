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

[l08u_brainlab] - Miracle Machine
- x162_st_snork - Basically the whole zone right after you enter the Miracle Machine. Previously DAO could spawn anomalies right on the ladder causing you to not be able to move forward.
