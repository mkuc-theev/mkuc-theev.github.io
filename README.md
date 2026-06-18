# The Official WTMC MCE2 Minecraft Server Client Setup Guide
<sub> *(TOWTMCMCE2MSCSG) for short* </sub>
## Some server information
**IP Address:** `mc.wokepikmin.army`\
**Minecraft version:** `1.20.1`\
**Mod loader:** Forge\
**Whitelist:** Enabled (bother `theev` on discord about getting whitelisted)\
**Modpack:** [MC Eternal 2](https://www.curseforge.com/minecraft/modpacks/mc-eternal-2)\
**Additional mods not in the pack:**
- [Simple Voice Chat](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/7905002)
- [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered/files/6352920)

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
2. Download the following files: [MCE2 (`.zip`)](https://www.curseforge.com/minecraft/modpacks/mc-eternal-2/files/8258389), [Simple Voice Chat (`.jar`)](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/7905002) and [Sound Physics Remastered (`.jar`)](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered/files/6352920).
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
   - Ctrl + click both the Simple Voice Chat and Sound Physics Remastered `.jar` files to select them, then click "Open"\
     <img width="80%" height="auto" alt="image" src="https://github.com/user-attachments/assets/e27162af-8070-431b-8557-0dcc43e7c044" />
   - The mods will be automatically installed and you can click "Close" on the remaining window. Your game is now ready to go.

# The next steps

In the Prism instance settings, go to the Java tab and under memory, set minimum and maximum memory usage such that they're both the same (recommended 8192 or 10238 MiB). Also, tick the "Java Arguments" box and paste in `-Xms10G -Xmx10G -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1`
\
## Game settings
Take time to fiddle with your game settings, especially stuff like shader quality, UI scale, better to have this stuff ready before the first session. Spin up a singleplayer world to make sure stuff works and runs well enough.
## Connecting to the server
It's dead simple. Click "Multiplayer", then "Add Server", put in whatever name you want in the "Server Name" field and `mc.wokepikmin.army` in the "Server Address" field. Click done, bob's your uncle.
## Voice chat
Once you're connected to the server and your character is created, you can press `V` to bring up the voice chat menu. The first time you do this it'll guide you through the first setup, simply do what it tells you to do. Or else.

# Frequently asked questions
### Q: Can I ask you the first question?
**A:** Yes.
