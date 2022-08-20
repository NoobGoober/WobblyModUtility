# WobblyModUtility
A Mod Loader For Wobbly Life

# Before You Use
What people do with this tool is outside our control. We do not encourage cheating in online play. All mods included in the program are checked for malware but mods downloaded from elsewhere are not our responsibility 

This program is not official and is not endorsed by the Wobbly Life developers

# Usage
1. Download and launch the program
2. On the to bar, select choose path and navigate to your installation of Wobbly Life (This will be saved for the future)
3. Select the mods you want to use (Select none to just install the modding framework to your game)
4. Press "Install / Update". You can check the status in the bottom left
5. Launch wobbly life as usual, it is recommended to quit and relaunch a couple of times for mods to work properly
6. Enjoy your modded Wobbly Life experience!

# Updating mods
If changes have happened to the game and mods need to be updated to work, or if you just want to enable / disable mods, simply press "Install /  Update" again and it will remove, add, or update all mods selected.

# Custom Mods
You can also install non verified mods from other sources. To do this, navigate to the "Add Custom Mod" tab ans pres the "Select mod DLL" file. In the prompt, select the mod and press open. The mod will be installed and a message will be displayed onscreen

> ⚠️ Be careful: Mods downloaded from unkown sources can contain malware, only get mods from people you trust! 

# Other tips and tricks

- Select "launch without mods" to launch the game with no mods active, whithout having to delete them!

- Select remove mods to go back to a clean installation of wobbly life!

# Creating Mods

Follow the melon loader documentation [here](https://melonwiki.xyz/#/modders/quickstart) to get your mod running. Next, to add support with the in game mod manager, add a refrence to "WobblyModMenu.dll" and add the namespace 'WobblyModLoader' to your script. At the start of all functions, add this code snippet, replacing "ModDLLFilename" with the name of your mods output file (EG: "MyCoolMod.dll") 

```if(!WMM.CanShowMod("ModDLLFilename")) {return;}```
