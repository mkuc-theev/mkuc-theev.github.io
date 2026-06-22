# The Official WTMC BMC3 Minecraft Server Client Setup Guide
<sub> *(TOWTMCBMC3MSCSG) for short* </sub>
## Some server information
**IP Address:** `mc.wokepikmin.army`\
**Minecraft version:** `1.21.1`\
**Mod loader:** Fabric\
**Whitelist:** Enabled (bother `theev` on discord about getting whitelisted)\
**Modpack:** [Better MC 3](https://www.curseforge.com/minecraft/modpacks/better-mc-fabric-bmc3/files/8051910)\
**Additional mods not in the pack:**
- [Simple Voice Chat](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/8293104)
- [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered/files/6352948)
- [Distant Horizons](https://www.curseforge.com/minecraft/mc-mods/distant-horizons/files/8287411) (Optional but highly recommended)
- [Oritech](https://www.curseforge.com/minecraft/mc-mods/oritech/files/8295561)
- [Reliable Backpacks](https://www.curseforge.com/minecraft/mc-mods/reliable-backpacks/files/8223384)
  
<sub> (don't worry, install instructions are below) </sub>\
\
The Minecraft server integrates with the `#minecwaft` channel on the discord, with a bot that provides server online status, player count, player joining/leaving/advancement notifications, and relays messages both ways between the discord channel and the in-game text chat.

## What you'll need to join us
- Minecraft (purchasable [here](https://www.minecraft.net/en-us/store/minecraft-java-bedrock-edition-pc?tabs=%7B%22details%22%3A0%7D))
- A Minecraft launcher ([Prism Launcher](https://prismlauncher.org/) is *highly* recommended and this guide is written with the assumption you're using it)
- A microphone* (highly recommended as most of our communications will use proximity VC, but not strictly needed)

# Getting your game set up
<sub> *Yes I know the screenshots show fantasia, I'm not retaking all of them, it's basically the same process, you're smart enough* </sub>
1. [Download](https://prismlauncher.org/) Prism from their website and install the program. Log into your Microsoft account. You'll be greeted with this window:
    <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/2cfef3ab-5229-48b2-b99d-ad234130c5ce" />
2. Download [Better MC 3](https://www.curseforge.com/minecraft/modpacks/better-mc-fabric-bmc3/files/8051910), [Simple Voice Chat](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/8293104), [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered/files/6352948), [Distant Horizons](https://www.curseforge.com/minecraft/mc-mods/distant-horizons/files/8287411) (if you want), [Oritech](https://www.curseforge.com/minecraft/mc-mods/oritech/files/8295561) and [Reliable Backpacks](https://www.curseforge.com/minecraft/mc-mods/reliable-backpacks/files/8223384).
3. Create your minecraft instance:
   - Click on "Add instance" in the top-left corner of the window\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/4f92dc51-0d9e-4754-ac14-064c2fc44156" />
   - On the left, select "Import", then click "Browse"\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/9c121c1f-efb4-4e48-ba31-eca8c70ca2d9" />
   - Navigate to where you downloaded Fantasia and double-click the file\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/9780ef21-963c-4d72-9369-ef0df006dd26" />
   - Optionally give your instance a custom name and click "Ok"\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/3c631903-16bf-4054-bbc2-c36ebb8733f6" />
   - You'll likely see this window pop up. Clicking the "Open missing" button will open several tabs in your browser. Clicking each tab will automatically start the downloads for the missing mods.\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/6892c4cc-4e33-4b2e-8260-a2e576fe5e2d" />
   - After the downloads are complete, return to Prism. It should say "All mods found" in the bottom-left corner. Click "Ok" to continue\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/7fa3af63-080c-49f0-9f86-e846928b7184" />
4. After the instance is created, let's add the rest of the mods.
   - Right-click the instance and select "Edit...". Navigate to "Mods" and click "Add file"\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/2251ef4e-1f67-409d-b0c7-7e4df4ffa07a" />
   - Ctrl + click both the Simple Voice Chat, Sound Physics Remastered, DH, Oritech, Reliable Backpacks and/or other applicable `.jar` files to select them, then click "Open"\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/e27162af-8070-431b-8557-0dcc43e7c044" />
   - The mods will be automatically installed and you can click "Close" on the remaining window. Your game is now ready to go.

# The next steps
## (Optional) Install Java 25
Newer java go brrr. This build is recommended by the MC optimization guide I found.\
1. Go [here](https://adoptium.net/) and click the download button. Run the installer. If you want Temurin to be your default JDK (honestly probably doesn't matter either way), select all the features to be installed on this screen.\
    <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/9c61bc68-8733-4945-8105-8b15fa621c02" />
2. Right click your MC instance, click `Edit...`, go to `Settings > Java`, tick the "Java Installation" box, then the `Detect` button. Select the entry that says "Adoptium" and click `Ok`. Additionally, tick the "Skip Java compatibility checks" box. (MC 1.21.1 is compatible with Java 25 but clients/loaders tend to yell at you for using it. If you encounter problems or simply don't want to push it, you can get the Java 21 version instead).\
    <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/6123c15b-d37e-4b28-876e-aaccc3abf7c5" />
3. Below, tick the "Memory" box. Set both minimum and maximum memory usage to the same value. (I suggest `8192 MiB` if you can spare it, `6144 MiB` if you can't). You can also set permgen to `256 MiB` but I'm not even certain that matters tbh.
4. Below, tick "Java Arguments" and paste this into the box: `-XX:+UseZGC -XX:+UseCompactObjectHeaders -XX:+UseStringDeduplication` (Distant Horizons doesn't like the default garbage collector and you'll get it yelling at you in in-game chat if you don't do this. If you have lots of memory and a weaker cpu, you can forgo string deduplication.)

## Game settings
Take time to fiddle with your game settings, especially stuff like shader quality, UI scale, better to have this stuff ready before the first session. Spin up a singleplayer world to make sure stuff works and runs well enough. The modpack has a lot of different shader presets, play around with them if you want.
## Connecting to the server
It's dead simple. Click "Multiplayer", then "Add Server", put in whatever name you want in the "Server Name" field and `mc.wokepikmin.army` in the "Server Address" field. Click done, bob's your uncle.
## Voice chat
Once you're connected to the server and your character is created, you can press `V` to bring up the voice chat menu. The first time you do this it'll guide you through the first setup, simply do what it tells you to do. Or else.
## Keybinds
Modpacks tend to have a lot of conflicting keybinds. Some to watch out for are `M` muting your voice comms when you try to open the map, or `V` doing random things when trying to configure the VC mod.

# Frequently asked questions
### Q: Can I ask you the first question?
**A:** Yes.
