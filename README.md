ALL Credits to [ryanrudolfoba](https://github.com/ryanrudolfoba)
# SteamOS Android Waydroid Installer

A collection of tools that is packaged into an easy to use script that is streamlined and tested to work with the Steam Deck running on SteamOS.
* The main program that does all the heavy lifting is [Waydroid - a container-based approach to boot a full Android system on a regular GNU/Linux system.](https://github.com/waydroid/waydroid)
* Waydroid Toolbox to easily toggle some configuration settings for Waydroid.
* [waydroid_script](https://github.com/casualsnek/waydroid_script) to easily add the libndk ARM translation layer and widevine.

**NOTE - this repository uses `main` and `testing` branches.**

**`testing`** - this is where new updates / features are pushed and sits for 1-2 weeks to make sure that bugs are squashed and eliminated. You can access it via this command (Temporary Link Until Original Repo returns) -
```
git clone --depth=1 -b testing https://github.com/Timbo303/steamos-waydroid-installer
```

**`main`** this is updated after 1-2 weeks in `testing` branch. You can access it via this command (Temporary Link Until Original Repo returns) -
```
git clone --depth=1 https://github.com/Timbo303/steamos-waydroid-installer
```

**Script has gone through several updates - this now allows you to install Android 11 / Android 13 and their TV counterparts - Android 11 TV / Android 13 TV!**

| [2026 SteamOS Waydroid Android Install Guide](https://www.youtube.com/watch?v=06T-h-jPVx8) | [SteamOS Waydroid Android Upgrade Guide](https://youtu.be/CJAMwIb_oI0) |
| ------------- | ------------- |
| [Android TV demo](https://youtu.be/gNFxrojouiM) | [Android 13 demo](https://youtu.be/5BZz8YynaUA) |

<details>
<summary><b>How to Access the Waydroid Folder in Dolphin File Manager</b></summary>

1. Launch Waydroid in Desktop Mode via konsole -
   cd ~/Android_Waydroid
   ./Android_Waydroid_Cage.sh
	
2. Wait for Waydroid to finish the boot sequence.

3. Launch Dolphin File Manager. In the address bar go to `/home/deck/.local/share/waydroid`
	<img width="750" height="349" alt="image" src="https://github.com/user-attachments/assets/97589bc7-7849-4d2f-91ce-ab100d710a9c" />

4. Right-click empty spot on the right pane and select `Open Dolphin File Manager as Root`
	<img width="985" height="602" alt="image" src="https://github.com/user-attachments/assets/7f39fbce-7a6d-40d1-979f-fb46f3b80785" />

5. Enter the sudo password when prompted
	<img width="956" height="470" alt="image" src="https://github.com/user-attachments/assets/9ca3d6c9-0d7a-42a2-bdf4-951eced81965" />

6. A new Dolphin File Manager will spawn that has root access
	<img width="779" height="321" alt="image" src="https://github.com/user-attachments/assets/aed41c5d-39c8-43a9-8437-dfacdc0d80d4" />

7. From here you can now access the Waydroid folders
	<img width="779" height="585" alt="image" src="https://github.com/user-attachments/assets/fc51f1b2-20f0-4720-b474-b4a50bfa72e3" />
</details>

> [!NOTE]
> If you are going to use this script for a video tutorial, PLEASE reference on your video where you got the script! This will make the support process easier!
> And don't forget to give a shoutout to [@10MinuteSteamDeckGamer](https://www.youtube.com/@10MinuteSteamDeckGamer/) / ryanrudolf from the Philippines!

<b> If you like my work please show support by subscribing to [YouTube channel @10MinuteSteamDeckGamer.](https://www.youtube.com/@10MinuteSteamDeckGamer/) </b> <br>
<b> I'm just passionate about Linux, Windows, how stuff works, and playing retro and modern video games on my Steam Deck! </b>

# Disclaimer
1. Do this at your own risk!
2. This is for educational and research purposes only!

# What's New (as of Feb 20 2026)
* change from Pixel 5 spoof to Pixel 10 Pro spoof
* ability to install custom LineageOS build that contains new fake wifi implementation (thanks ayesa)
* fake wifi config automatically enabled for PvZ 2
* latest ATV13 builds (thanks supechicken)
* workaround for small var partition in SteamOS - ability to use libhoudini
* libhoudini as default translation layer instead of libndk for greater compatibility (pokemon, arknights, fire emblem etc are working) (thanks gagantous for the initial testing)
* fix for intermittent broken internet
* k2er, mantis, shizuku automatic activation
* CoD Mobile controller support (thanks Wudi-ZhanShen)
* maybe something else i forgot to write!

thanks to waydroid devs, ayesa, supechicken, Wudi-ZhanShen, gagantous and casualsnek!

<details>
<summary><b>Old Changelog - Click here for more details</b></summary>
**What's New (as of Nov 15 2025)**
1. Xbox Wireless Controller spoofing so that Call of Duty CoD Mobile works with the Steam Deck controller
2. Fixed low audio on fresh install
3. Latest StevenBlack adblock host file automatically downloaded during install
4. Added logic to the shizuku and mantis activation
5. Improved Decky Loader sanity check
6. Implemented logging
7. Refactored the python script that adds the waydroid icon for easy readability of the script
8. Updated uninstall

**What's New (as of July 28 2025)**
1. Sanity check updated - instead of kernel version check it will check if running on SteamOS stable / SteamOS beta
2. Auto build the binder kernel module
3. Cleanup and remove traces of A11. Available options to choose - A13 GAPPS, A13 NO_GAPPS, ATV13 NO_GAPPS

**What's New (as of July 02 2025)**
1. Support for SteamOS stable 3.7.13 (this is same kernel used as 3.7.10 so really nothing changed here)

**What's New (as of June 19 2025)**
1. Support for SteamOS beta 3.7.10

**What's New (as of June 03 2025)**
1. `testing` branch works on latest SteamOS stable 3.7.8 and latest SteamOS beta 3.7.9.
2. Updated waydroid from 1.4.3 to 1.5.1
3. Updated official Android 13 GAPPS / NOGAPPS image. This uses latest build as of May 31 2025

**What's New (as of May 16 2025)**
1. Official Android 13 images (GAPPS and NOGAPPS)
2. Working LIBNDK ARM translation layer for Android 13

**What's New (as of Feb 28 2025)**
1. Spoof Android TV to Philips TV

**What's New (as of Jan 21 2025)**
1. Initial support for Android 13 - NOGAPPS

**What's New (as of Jan 20 2025)**
1. Initial support for Android 13 TV

**What's New (as of Jan 16 2025)**
1. Initial support for Android 11 TV

**What's New (as of Dec 27 2024)**
1. Support for SteamOS Beta 3.6.21
2. Uploaded initial Waydroid Android 11 TV image in the [release section](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/releases/tag/Android11TV)

**What's New (as of Oct 28 2024)**
1. Support for latest SteamOS Stable 3.6.19
2. fixed binder kernel module parameters
3. enhancement - ability to choose with / without Google Playstore on a fresh install
4. enhancement - automatically activate mantis gamepad pro and shizuku
5. enhancement - disable root detection (some apps might still detect root)
6. enhancement - disable first time setup wizard
7. enhancement - Waydroid Toolbox - added NETWORK option
8. enhancement - Waydroid Toolbox - updated ADBLOCK option

**What's New (as of Oct 10 2024)**
1. add support for latest SteamOS Beta 3.6.16 / 3.6.17
2. add sanity check for home and var partition - make sure home has at least 5GB free space, and var has at least 100MB free space
3. add / fix verbose messages
4. trim output of steamos-add-to-steam

**What's New (as of Sep 07 2024)**
1. support for SteamOS 3.6.12

**What's New (as of Aug 27 2024)**
1. support for SteamOS 3.6.10
2. added experimental waydroid launcher that supports rotation - [demo here](https://youtu.be/OxApPDhZn9I)
3. Waydroid Toolbox - option to uninstall waydroid and retain android user data, or full uninstall of waydroid including android user data

**What's New (as of Aug 09 2024)**
1. support for SteamOS 3.6.9
2. waydroid bump from 1.4.2 to 1.4.3
3. lxc bump from 0.2 to 0.3
4. binder kernel module re-built using latest May26 commits
5. cleanup the binder kernel folder names so its easier to read
6. remove libndk-fixer (not needed anymore for Roblox)
7. Add sanity check on the waydroid launcher

**What's New (as of May 28 2024)**
1. Fix for scoped storage permission issue. Apps can now write to data / obb folder. [FIFA 14 now works because of this!](https://youtu.be/_10oQK-ionY?si=bfIBvHPv_spyLPCy)

**What's New (as of May 05 2024)**
1. Minor fix - make minigbm_gbm_mesa as default. This should make [Roblox performance better.](https://youtu.be/-czisFuKoTM?si=8EPXyzasi3no70Tl)
2. Waydroid Toolbox - added option to toggle between gbm or minigbm_gbm_mesa.
3. Added verbose error message when Waydroid initialization fails during install.

**Updated Waydroid Toolbox to easily configure some aspects of Waydroid**
![image](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/assets/98122529/3973f218-25a4-4e4b-aba6-b96c45f9a4ef)

**What's New (as of May 01 2024)**
1. Roblox now works thanks to slappy826! [demo guide here how to configure Roblox](https://youtu.be/-czisFuKoTM?si=8EPXyzasi3no70Tl)
2. Updated the Waydroid Toolbox script
3. code cleanup / additional logic
4. switch from gbm to minigbm_gbm_mesa

**What's New (as of April 25 2024)**
1. This works with latest stable SteamOS 3.5.19. There is no kernel change for SteamOS - it still uses 6.1.52-valve16-1 so this works right away no need for new kernel modules.\
SteamOS has been stuck on 6.1.52-valve16-1 for several releases now so I think this will stay and next major bump will be on SteamOS 3.6.x.

**What's New (as of March 09 2024)**
1. Updated launcher to easily run APKs in Game Mode. [demo guide here](https://youtu.be/pkRtPHfa_EM?si=broimKF1menbRxGg)
2. Fix minor typo in uninstall - this now removes the Waydroid application entries in the KDE menu.
3. Added Waydroid Toolbox to easily configure some aspects of Waydroid.
![image](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/assets/98122529/058c1321-4636-44d7-8b7d-1569f478894b)

**What's New (as of February 11 2024)**
1. Added support for latest SteamOS Preview 3.5.15 - kernel 6.1.52-valve16-1-neptune-61

**What's New (as of February 10 2024)**
1. [lower audio latency](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/issues/22)
2. added more sanity checks

**What's New (as of February 07 2024)**
1. removed weston. been testing cage for several weeks now and this is way better than weston.
2. added custom hosts file to block ads

**What's New (as of February 05 2024)**
1. merged PR - [Add fixed key layout file for Steam Deck controller](https://github.com/ryanrudolfoba/SteamOS-Waydroid-Installer/pull/19)
2. SteamOS 3.5.14 works. No need to recompile kernel module as it uses the same kernel from 3.5.13

**What's New (as of February 02 2024)**
1. added cage launcher for multi-touch support
2. rewrite the script - instead of building from source this now installs prebuilt binaries
3. easier and quicker to install
4. added support for SteamOS 3.5.13 Preview

**What's New (as of December 07 2023)**
1. this now works with [casualsnek script!](https://github.com/casualsnek/waydroid_script)
2. added libndk arm translation layer (via casualsnek script)
3. added widevine (via casualsnek script). This is needed for Netflix and Disney+
4. waydroid fingerprint identifies as a [Pixel 5 redfin.](https://github.com/Quackdoc/waydroid-scripts) This is needed for Netflix
5. new method for detecting controller [via Saren method](https://gist.github.com/Saren-Arterius/c5bc39199552a5c244449b0ce467d6b6)

**What's New (as of November 26 2023)**
1. cleanup and removed support for SteamOS 3.4.x due to SteamOS 3.5.x already went to stable
2. removed PlasmaNested.sh as this is already included in SteamOS 3.5.x
3. removed the bundled weston binary (only useful when on SteamOS 3.4.x)

**What's New (as of November 15 2023)**
1. initial release
</details>

# Install Steps
<details>
<summary><b>Click here - Read the sections below carefully for steps on how to install and use this script!</b></summary>

**Prerequisites for SteamOS**
1. `sudo` password should already be set by the end user. If `sudo` password is not yet set, the script will ask to set it up.

**How to Use and Install the Script**
1. Go into Desktop Mode and open a `konsole` terminal.
2. Clone the github repo.
	To clone the `main` branch -
   ```sh
   cd ~/
   git clone --depth=1 https://github.com/Timbo303/steamos-waydroid-installer
   ```

	To clone the `testing` branch where new features / updates are being tested before it goes to `main` -
	```sh
   cd ~/
   git clone --depth=1 -b testing https://github.com/Timbo303/steamos-waydroid-installer
   ```

3. Execute the script! \

   ```sh
   cd ~/steamos-waydroid-installer
   chmod +x steamos-waydroid-installer.sh
   ./steamos-waydroid-installer.sh
   ```

4. Script will automatically install Waydroid together with the custom config. Install will roughly take around 5mins depending on the internet connection speed.
5. Once done exit the script and go back to Game Mode.

**Launching Waydroid**
1. Go to Game Mode.
2. Run the Android_Waydroid_Cage launcher.
</details>

# Additional Considerations
<details>
<summary><b>Click here - Read the sections below carefully. These are purely OPTIONAL.</b></summary>

**Steam Deck Controller Layout**
Thanks to DanielLester83!

Search 'Waydroid' in the community templates or maybe this link would work steam://controllerconfig/3665077347/3304296813

This maps the back buttons to function keys for use with android key remappers like this https://github.com/keymapperorg/KeyMapper

This work around seems to be needed because steaminput does not seem to pass the Search/OS/Windows/Meta Key to Android.

This layout also tweaks the trackpad inputs.

**Configure Android Start Menu Shortcuts to Work in Desktop Mode** \
Work in Progress. Thanks to DanielLester83 for the instructions!

**Controller Not Being Detected** \
The script has been updated so that the controller detection will get triggered once Android has completed the boot process. This makes the controller detection more accurate and the boot sequence to be faster.

</details>

# I dont want this anymore! I want to uninstall!
1. Go to Desktop Mode.
2. There will be an icon called Waydroid Toolbox on the desktop.
3. Launch that icon and select UNINSTALL.

# Troubleshooting / Filing Bug Reports
1. If you encounter an issue with the script, try to [uninstall](https://github.com/Timbo303/SteamOS-Waydroid-Installer/tree/main#i-dont-want-this-anymore-i-want-to-uninstall), clone the repo again and perform an install.\
Reason for that - you might be using an older version of my script and a new version might have already fixed your issue.
2. If uninstall / reinstall didn't help, open an issue and please be descriptive as possible. \
At the minimum include this when filing an issue - \
SteamOS version - \
Error message encountered - \
Screenshot of error - \
Do you have any scripts / tweaks that might be causing issues?
3. Downloads are slow when acquiring the waydroid image. \
Answer - You might have connected to a slow sourceforge mirror. Press CTRL-C to cancel the download and re-run the script again.
4. No shortcuts in Game Mode after running the script / Unsupported File Type when adding shortcuts. \
Answer - This issue happens if Steam client cant be run because the script was called from an ssh or virtual tty session. Make sure to run the script on Desktop Mode via konsole.

# A Note on SteamOS Updates
When there is a SteamOS update the waydroid will be wiped. This is normal behavior due to how SteamOS applies updates. \
Re-run the script again but if the SteamOS update contains a new kernel version the script will exit immediately. \
Please file an issue report when this happens so I can compile a binder kernel module to match the SteamOS update.

# Mini-guides for Steam Deck Android Waydroid
These mini guides are tailor-fitted for the Steam Deck that uses the script provided in this repo. WIP

# Games Tested By Me on Android Waydroid Steam Deck
[Geekbench Benchmark Result Between Steam Deck OLED and Steam Deck LCD on SteamOS Android Waydroid](https://youtu.be/56YGZsU5j74) - Feb 11 2024 \
[Plants vs Zombies](https://youtu.be/rnb0z1LtDN8) - Feb 04 2024 \
[Honkai Star Rail](https://youtu.be/M1Y9DMG9rbM) - Feb 06 2024 \
[Asphalt 8 Airborne](https://youtu.be/OCaatZdZR1I) - Feb 08 2024 \
[Honkai Impact 3rd](https://youtu.be/6YdNOJ0u2KM) - Feb 10 2024 \
[Mobile Legends](https://youtu.be/PlPRNn92NDI) - Feb 13 2024 \
[T3 Arena](https://youtu.be/wq87nd3MCrQ?si=h4A7NEwEFGujF7hH) - Feb 16 2024 \
[Warcraft Rumble](https://youtu.be/rnb0z1LtDN8) - Feb 19 2024 \
[Diablo Immortal](https://youtu.be/4lJOnGnEJjw) - Feb 21 2024 \
[Oceanhorn](https://youtu.be/vKPJZeyw0DI) - Feb 23 2024 \
[Candy Crush Saga](https://youtu.be/XEcIYBDoOZk) - Mar 11 2024 \
[BombSquad](https://youtu.be/vatf5uY_Eak) - Mar 16 2024 \
[Project BloodStrike](https://youtu.be/pRwvZBMDpY0) - Mar 18 2024 \
[NBA Infinite](https://youtu.be/LLw4GnWL58I) - Mar 23 2024 \
[Roblox](https://youtu.be/-czisFuKoTM?si=8EPXyzasi3no70Tl) - May 01 2024 \
[Plants vs Zombies 2 - Reflourished](https://youtu.be/RurH-XTTSDQ) - May 17 2024 \
[Wuthering Waves](https://youtu.be/KfQVCTtpiNI) - May 23 2024 \
[FIFA 14](https://youtu.be/_10oQK-ionY?si=bfIBvHPv_spyLPCy) - May 28 2024 \
[KOF Arena / King of Fighters Arena](https://youtu.be/XlIB9MwyQdw?si=zLa5AAPyrAXiKct8) - June 18 2024 \
[Injustice](https://youtu.be/fMG4OMhcpz8) - July 12 2024 \
[Wuthering Waves using patched LIBNDK](https://youtu.be/vBRFzg14Sp4) - Aug 01 2024 \
[Roblox x86 APK](https://youtu.be/8lDD7mQYEas) - Aug 03 2024 \
[Blue Archive using patched LIBNDK](https://youtu.be/WtUluvNznpA) - Aug 27 2024

# Games Tested by Other Users
Please check this [google sheets](https://docs.google.com/spreadsheets/d/1pyqQw2XKJZBtGYBV0i7C510dyjVSU2YndhaTOEDavdU/edit?usp=sharing) for games tested by other users. \
If you wish to contribute, please include the game name, how it runs etc etc. \
Please feel free to add your game testing in there too! Thank you!
