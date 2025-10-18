# Gear VR Controller Motion Pointer for Windows

<img src="./screenshot.png" alt="Screenshot" style="width:765px; height:auto;">

[Deutsch](https://shimuraworksh.wixsite.com/shimura-workshop/de/s-projects-side-by-side)
[Español](https://shimuraworksh.wixsite.com/shimura-workshop/es/s-projects-side-by-side)
[Français](https://shimuraworksh.wixsite.com/shimura-workshop/fr/s-projects-side-by-side)
[Italiano](https://shimuraworksh.wixsite.com/shimura-workshop/it/s-projects-side-by-side)
[日本語](https://shimuraworksh.wixsite.com/shimura-workshop/ja/s-projects-side-by-side)
[한국어](https://shimuraworksh.wixsite.com/shimura-workshop/ko/s-projects-side-by-side)
[Português](https://shimuraworksh.wixsite.com/shimura-workshop/pt/s-projects-side-by-side)
[中文](https://shimuraworksh.wixsite.com/shimura-workshop/zh/s-projects-side-by-side)

Convert the 37g lightweight VR controller into a powerful PC gadget

Features
- No VR headset or mobile phone needed
- Wireless presenter, air mouse and motion pointer
- Emulated light gun, gyro and motion gamepad
- Key or action mapping to buttons and motions
- Combo editor for keys input
- Trackpad mouse cursor or scrolling
- Compass mode
- Quick and easy calibration of sensors

Setup guide
- No manual pairing needed, just turn on PC Bluetooth and install batteries to the controller
- Press any button on the controller, then click the Search icon in app
- Click the Connect button, that's it

Calibration for motion sensing and motion pointer
- Place the controller upside down on a stable surface, then click the CAL button, that's it

Download latest version

- v2.2.0 [Link](https://www.mediafire.com/file/mr4r299a5cj822j/Gear_VR_Controller_setup.exe/file)
- md5: f1b921deeaf0bbdf0e60673b7e6b4663
- sha-1: 694fe2b6fb66f26c5d4d69e3a386988f2c46f163

System requirements
- Windows 10 x64 or Windows 11
- [.NET Desktop Runtime 9.0](https://dotnet.microsoft.com/download/dotnet/9.0)

[Major change log](https://github.com/ShimuraWorkshop/Gear-VR-Controller-Motion-Pointer-for-Windows/wiki#major-change-log)

[Troubleshooting](https://github.com/ShimuraWorkshop/Gear-VR-Controller-Motion-Pointer-for-Windows/wiki#troubleshooting)

<br>

Details
- [\*Secret\* gyro/motion gamepad emulation](#secret-gyromotion-gamepad-emulation)
- [Lightgun emulation](#lightgun-emulation)
- [Gyro aiming for rail shooter games](#gyro-aiming-for-rail-shooter-games)
- [Pairing 2 or more Gear VR controllers *\*\*New\*\**](#pairing-2-or-more-gear-vr-controllers)
- [Lightgun input using DemulShooter](#lightgun-input-using-demulshooter)
- [< The House of the Dead 2: Remake > PC gyro aiming](#-the-house-of-the-dead-2-remake--pc-gyro-aiming)
- [< The House of the Dead: Remake > PC gyro/lightgun aiming](#-the-house-of-the-dead-remake--pc-gyrolightgun-aiming)
- [< Panzer Dragoon: Remake > PC gyro aiming](#-panzer-dragoon-remake--pc-gyro-aiming)
- [< Blue Estate The Game > PC lightgun aiming](#-blue-estate-the-game--pc-lightgun-aiming)
- [< The Typing of the Dead: Overkill > PC lightgun aiming](#-the-typing-of-the-dead-overkill--pc-lightgun-aiming)
- [< The House of the Dead III > PC lightgun aiming](#-the-house-of-the-dead-iii--pc-lightgun-aiming)
- [< The House of the Dead 2 > PC lightgun aiming](#-the-house-of-the-dead-2--pc-lightgun-aiming)
- [< House of the Dead: Scarlet Dawn > PC lightgun aiming](#-house-of-the-dead-scarlet-dawn--pc-lightgun-aiming)
- [< MAME > emulator PC lightgun aiming (for Virtua Cop, Time Crisis, Alien 3: The Gun, etc)](#-mame--emulator-pc-lightgun-aiming)
- [< Cxbx-Reloaded > emulator PC lightgun aiming (for Virtua Cop 3, Silent Scope 2)](#-cxbx-reloaded--emulator-pc-lightgun-aiming)
- [< TeknoParrot > emulator PC lightgun aiming (for Time Crisis 5, Operation GHOST, etc)](#-teknoparrot--emulator-pc-lightgun-aiming)
- [< RPCS3 > emulator PC lightgun aiming (for Time Crisis: Razing Storm, etc)](#-rpcs3--emulator-pc-lightgun-aiming)
- [< PCSX2 > emulator PC lightgun aiming (for Time Crisis 3, Vampire Night, etc)](#-pcsx2--emulator-pc-lightgun-aiming)
- [< DuckStation > emulator PC lightgun aiming (for Time Crisis: Project Titan, Point Blank 3, etc)](#-duckstation--emulator-pc-lightgun-aiming)
- [< Dolphin > emulator PC lightgun aiming (for Ghost Squad, The House of the Dead: Overkill, etc)](#-dolphin--emulator-pc-lightgun-aiming)
- [< Snes9x > emulator PC lightgun aiming (for Yoshi's Safari, etc)](#-snes9x--emulator-pc-lightgun-aiming)
- [< FCEUX > emulator PC lightgun aiming (for Duck Hunt, etc)](#-fceux--emulator-pc-lightgun-aiming)
- [< Flycast > emulator PC lightgun aiming (for Confidential Mission, Ninja Assault, etc)](#-flycast--emulator-pc-lightgun-aiming)
- [< Supermodel > emulator PC lightgun aiming (for The Lost World: Jurassic Park, etc)](#-supermodel--emulator-pc-lightgun-aiming)
- [< Demul > emulator PC lightgun aiming (for Brave Firefighters, etc)](#-demul--emulator-pc-lightgun-aiming)
- [Backup of user config](#backup-of-user-config)
- [Hints on low input lag](#hints-on-low-input-lag-for-games-and-emulators)

<br>

Gear VR is a trademark or registered trademark of Samsung Electronics Co., Ltd.
<br>
Windows is a trademark or registered trademark of Microsoft Corporation

<br>

## \*Secret\* gyro/motion gamepad emulation

You can use the controller like a gyro gamepad, with analog touch stick (needn't press) and gyro aiming support. Gamepad buttons and sticks are available in key assignment list for mapping to touchpad press (4 directions, center and lower edge), other 5 buttons and 12 motion gestures.

To use the gamepad mode, install [ViGEmBus](https://github.com/nefarius/ViGEmBus/releases/tag/v1.22.0), edit the file "C:\Program Files\Gear VR Controller\Gear_VR_Controller.dll.config" (default, text editor needs to be run as admin) and restart the app.

Modify this option from True to False:

DefaultStabilizePointerClick

Modify these options from False to True:

DefaultGameMode
<br>
DefaultGameKeyboardMode
<br>
DefaultGamePointerMode
<br>
DefaultEmulateGamepad

Adjust the motion pointer speed to around 1~4 in app and switch to motion pointer mode before starting game. Also adjust the cursor speed in Windows mouse settings when necessary. For easier control, assign "Toggle between cursor and pointer mode" or "Pointer temporary off" to a button. For gyro activation with another action, you can assign "Pointer temporary on" to the second action of buttons by modifying any of these options:

KeyTouchButtonCenter2 / KeyBackButton2 / KeyHomeButton2 / KeyVolumeUpButton2 / KeyVolumeDownButton2 / KeyTouchButton2 / KeyTriggerButton2 / KeyTouchDirectCenter2

You can also map controller roll, pitch, yaw motions to stick axes or triggers to make it a motion gamepad. Adjust the motion pointer speed to around 1~3 and assign "Pointer reset" to a button. Explore more settings if you're interested.

Modify these options from False to True:

DefaultGamepadUsePitch
<br>
DefaultGamepadUseYaw

Some games may work better with keyboard+mouse emulation, or if you want to use mixed input with another gamepad, in that case, leave the DefaultEmulateGamepad option to False.

If the game is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

<br>

## Lightgun emulation

### Option 1: Lightgun emulation replacing mouse

Config file [Link](https://www.mediafire.com/file/nr93jqt7o9zzsg4/Gear_VR_Controller.dll.config_lightgun.zip/file) (if supported by the game or emulator)

ViGEmBus not required, update the app to v2.2.0, unzip the config to "C:\Program Files\Gear VR Controller" (default).

Assign "Pointer reset" to Touchpad South, "Mouse left button" to Trigger, also other keys to suit the game. Adjust the motion pointer speed to around 8~12 in app and switch to motion pointer mode before starting game.

### Option 2: Lightgun emulation replacing gamepad stick

Config file [Link](https://www.mediafire.com/file/lo7iu6lflxh00hl/Gear_VR_Controller.dll.config_lightgun.by.gamepad.zip/file) (if supported by the game or emulator)

Install [ViGEmBus](https://github.com/nefarius/ViGEmBus/releases/tag/v1.22.0), update the app to v2.2.0, unzip the config to "C:\Program Files\Gear VR Controller" (default).

Assign "Pointer reset" to Touchpad South, "Gamepad A" to Trigger, also other keys to suit the game. Adjust the motion pointer speed to around 8~12 in app for the game.

With either config, if the game or emulator is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

<br>

## Gyro aiming for rail shooter games

Config file [Link](https://www.mediafire.com/file/t7shxu9czk3wdj1/Gear_VR_Controller.dll.config_gyro.zip/file) (if supported by the game or emulator)

ViGEmBus not required, update the app to v2.2.0, unzip the config to "C:\Program Files\Gear VR Controller" (default).

Assign "Pointer temporary off" to Touchpad South, "Mouse left button" to Trigger, also other keys to suit the game. Adjust the motion pointer speed to around 4 in app and switch to motion pointer mode before starting the game. Also adjust the cursor speed in Windows mouse settings when necessary.

Mouse acceleration will be disabled by default, the original state will be restored after exiting the app.

If the game or emulator is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

<br>

## Pairing 2 or more Gear VR controllers

By default, only a single Gear VR controller can be paired with Windows. To make it possible to pair 2 or more Gear VR controllers at the same time, you need to modify the hard-coded Bluetooth IRK of the existing controller in Windows registry.

A maximum of 4 gamepad-based controllers plus 1 mouse-based controller can work at the same time, depending on the support by games or emulators. For example, in TeknoParrot, 4 gamepad-based controllers can be set. In PCSX2, DuckStation, Dolphin and Flycast, both mouse-based and gamepad-based controllers can be set for players. In MAME, multiple gamepad-based controllers are set for different players by default. For games supported by DemulShooter input, 4 gamepad-based controllers can be set as light guns input.

Beware that modifying the registry incorrectly may make your Windows corrupt, do it at your own risk.

Procedures:
1. Update the app to v2.2.0.
2. Make a note of the MAC address of existing Gear VR controller from the lower left corner of the app.
3. Disconnect the controller and exit the app.
4. Download and unzip [PSTools](https://docs.microsoft.com/en-us/sysinternals/downloads/psexec).
5. In Windows command prompt with admin privilege, go to the folder of unzipped files, run "psexec64 -s -i regedit".
6. In regedit, go to the folder "\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\BTHPORT\Parameters\Keys".
7. Inside "Keys" folder, go to the sub-sub folder with the folder name same as the MAC address of the existing Gear VR controller.
8. Modify the "IRK" data, the original value should be "01 23 45 ...". Change the first byte from "01" to "02", and make sure to delete "01", not just insert new byte. If you're using more than 2 Gear VR controllers, change to "03" or "04", etc, as long as there's no duplicate IRK and not keeping the original "01".
10. Click OK to save, exit regedit, and restart the computer.
11. Make a copy of the Gear VR Controller app folder with all contents ("C:\Program Files\Gear VR Controller" by default), with a new folder name e.g. "Gear VR Controller P2".
12. Make sure only the new controller is powered on by removing batteries from other controllers. Don't pair the controller manually in Windows bluetooth settings.
13. Start the new copy of app and setup the new controller as usual. A new set of user config will be created in "%LOCALAPPDATA%\Gear_VR_Controller".
14. Start other copies of app as usual. Multiple instances of the app in different folders can be run at the same time. The order of XInput device ID will be according to the order of starting instance of the app.

<br>

## Lightgun input using DemulShooter

[DemulShooter](https://github.com/argonlefou/DemulShooter/releases) allows using up to 4 gamepad-based controllers to input as light guns to some games or emulators.

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Touchpad Center: Gamepad B, Touchpad North: Gamepad X, Touchpad South: Pointer reset

Run DemulShooter_GUI, in Page Selection, select the Configuration for each active player (P1, P2, etc). Set the Device to [Gamepad] [Unknown Manufacturer] - Controller (XBOX 360 For Windows), and test the corresponding controller on the GUI.

DemulShooter has light gun buttons assignment for Trigger, Off-Screen and Action Button only. For other keys of the game (e.g. Coin, Start, Up, Down, etc), you can assign them to other buttons of the controller in app.

See the [Wiki](https://github.com/argonlefou/DemulShooter/wiki/Usage) for supported games and detailed settings. Note that for some games, only output (LED, force feedback, etc) is supported by DemulShooter, but not input. Therefore, there is no effect to use it with the controller for those games.

DemulShooter.exe and DemulShooterX64.exe need to be run as admin or run in Windows command prompt with admin privilege.

<br>

## < The House of the Dead 2: Remake > PC gyro aiming

Follow the instructions of [gyro aiming](#gyro-aiming-for-rail-shooter-games), and assign keys for example:

Trigger: Mouse left button, Back: Enter, Home: Tab, +: F, -: Esc
<br>
Touchpad - Center: Mouse right button, West: Q, East: E, North: Unassigned, South: Pointer temporary off

In game options, set controller to Keyboard/Mouse, aiming stick to Both Sticks, mouse sensitivity to 1.0, crosshair speed to 1.0.

<br>

## < The House of the Dead: Remake > PC gyro/lightgun aiming

For gyro aiming, follow the [instructions](#gyro-aiming-for-rail-shooter-games), and assign keys for example:

Trigger: Mouse left button, Back: Enter, -: Esc
<br>
Touchpad - Center: Mouse right button, West: Q, East: E, North: F, South: Pointer temporary off

If you have installed a lightgun or arcade plugin (like [this](https://steamcommunity.com/app/1694600/discussions/0/3271312219438716734/) or [this](https://github.com/argonlefou/HotdRemake_ArcadePlugin/)), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and change the key assignments according to the plugin.

With either config, in game options, set controller type to Keyboard/Mouse, sensitivity to 1.0, crosshair speed to 1.00 (some settings may be unavailable in arcade plugin).

For 2-player support by using 2 Gear VR controllers, see [DemulShooter](#lightgun-input-using-demulshooter).

<br>

## < Panzer Dragoon: Remake > PC gyro aiming

Follow the instructions of [gyro aiming](#gyro-aiming-for-rail-shooter-games), and assign keys for example:

Trigger: Mouse left button, Back: Enter, Home: Esc, +: R, -: F
<br>
Touchpad - Center: Mouse right button, West: Q, East: E, North: Unassigned, South: Pointer temporary off
<br>
Non-Press Touchpad - West: A, East: D, North: W, South: S

In game options, set Crosshair Sensitivity to 1.00. Due to forced mouse smoothing used by the game, you need to move the controller slowly.

<br>

## < Blue Estate The Game > PC lightgun aiming

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game. In game's Controls settings, switch controller to Mouse, set Mouse in Raw Mode to Yes, Gestures with the Mouse to Yes.

<br>

## < The Typing of the Dead: Overkill > PC lightgun aiming

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game.

<br>

## < The House of the Dead III > PC lightgun aiming

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game.

For 2-player support by using 2 Gear VR controllers, see [DemulShooter](#lightgun-input-using-demulshooter).

<br>

## < The House of the Dead 2 > PC lightgun aiming

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game. In game's config, select Mouse + Keyboard for player controller.

For 2-player support by using 2 Gear VR controllers, see [DemulShooter](#lightgun-input-using-demulshooter). Use Enter and Tab for start buttons of P1 and P2, Up/Down arrow for menu navigation.

<br>

## < House of the Dead: Scarlet Dawn > PC lightgun aiming

For TeknoParrot, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Back/View
<br>
Touchpad - West: Gamepad LB, North: Gamepad X, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to XInput, uncheck General - Windowed, check General - HideCursor, check Crosshairs - Enable Native. In controller setup, set the mapping by pressing the buttons on Gear VR controller. For easier input during setup, set motion pointer speed to 1 and dead zone to 10000 in app. Then for Player 1, set Start by pressing Back, Gun Trigger by Trigger, Sub Trigger by Touchpad North, Controller Select by Touchpad West. Set dead zone back to 15 (default) and press Touchpad South to reset stick. Then set Player 1 Gun X by pointing the controller rightward slowly until X+ is shown, set Gun Y by pointing upward until Y+ is shown.

Adjust the motion pointer speed to around 8~12 for the game.

<br>

## < MAME > emulator PC lightgun aiming

### Option 1: Lightgun emulation replacing mouse (e.g. Time Crisis, Virtua Cop)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 5
<br>
Touchpad - Center: Mouse right button, North: Mouse middle button, South: Pointer reset

In MAME game's Input Device Options, set Lightgun Device Assignment to lightgun, Pedal Device Assignment to lightgun, Keyboard Input Provider to dinput, Lightgun Input Provider to win32.

Press Alt-Enter to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio.

If you want to use non-press touchpad for pedal, assign Mouse right button to Non-Press Touchpad Center.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Alien 3: The Gun)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: 1, Home: 5
<br>
Touchpad - Center: Gamepad B, North: Gamepad X, South: Pointer reset

Press Touchpad South to reset stick. In MAME game's Input Device Options, set Keyboard Input Provider to dinput, Joystick Input Provider to xinput. In Advanced Options, set Joystick to On, Joystick deadzone to 0, Joystick saturation to 1.

Press Alt-Enter to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio.

For some games like Terminator 2: Judgment Day which need to calibrate the gun for player 2, if not playing, press keyboard key A (default for player 2's gun trigger) to pass.

With either config, press Tab, select Crosshair Options, set Visibility to Always or Never when necessary (maybe unavailable in some games). Calibrate the gun crosshair in the game's Service and Test menu.

<br>

## < Cxbx-Reloaded > emulator PC lightgun aiming

For Virtua Cop 3, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad B (for Reload during ES Mode), Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B (for Reload), West: Gamepad X (for Weapon Change), North: Gamepad LT (for ES Mode), South: Pointer reset

In Cxbx-Reloaded's Input settings, select MS Gamepad S, click Configure. Set Device to XInput/0/Gamepad, click Default Bindings. Give the Profile a name and Save. In Video settings, set Display Resolution to your screen resolution and refresh rate, uncheck Use Exclusive Fullscreen Mode, check Maintain Aspect Ratio, and check Force VSync. Rename the file boot.id to something else in the root folder of game if existing.

Open the game by vc3.xbe, start emulation. Press Alt-Enter to switch to fullscreen. As the game is 4:3, if your screen's resolution is 16:9, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio. Due to the curved crosshair movement used by the game, aim will have some distortions especially at corners of the screen.

For Silent Scope 2 (in Silent Scope Complete), select EMS TopGun II in Input settings, use Default Bindings. Assign Gamepad RS Button to a button/motion to hide Laser dot in game, also assign Gamepad D-pad Up/Down/Left/Right to buttons/motions for menu navigation when necessary.

<br>

## < TeknoParrot > emulator PC lightgun aiming

(Most games work better with option 2)

### Option 1: Lightgun emulation replacing mouse

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 5
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to RawInput, uncheck General - Windowed, check General - HideCursor, check Crosshairs - Enable, check Crosshairs - Scaling (some settings may be unavailable in some games). In controller setup, set the mapping by pressing the buttons on Gear VR controller, and set Light Gun to Unknown Device.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Time Crisis 5)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Back/View, Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B, North: Gamepad X, West: Gamepad LB, East: Gamepad RB, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to XInput, check Crosshair - Enable, uncheck General - Windowed. In controller setup, set the mapping by pressing the buttons on Gear VR controller. For easier input during setup, set motion pointer speed to 1 and dead zone to 10000 in app, then set Coin by pressing Home, Gun Trigger by Trigger, Gun Button by Touchpad North, Left Pedal by Touchpad West, Right Pedal by Touchpad East. Set dead zone back to 15 (default) and press Touchpad South to reset stick, then set Player 1 Gun X by pointing the controller rightward slowly until X+ is shown, set Gun Y by pointing upward until Y+ is shown.

Adjust the motion pointer speed to around 8~12 for the game.

For Operation GHOST, check General - Windowed in game settings, and patch the game to correct screen resolution by [OpGhost_ResChanger](https://forum.arcadecontrols.com/index.php/topic,149714.msg1673148.html#msg1673148). Set max frame rate to 60 fps for the game (gs.exe) in GPU driver when necessary. If your version of game has the crosshair removed, try to restore the backup folder ".\root\img\UI\UI_hud_common.crosshair" if available.

For Rabbids Hollywood, if the crosshair or trigger doesn't work, maybe your version of game has a non-working trigger fix or Unity Plugin installed. Try to restore the backup file ".\Game_Data\Managed\Assembly-CSharp.dll.original" if available, also rename the file ".\winhttp.dll" to something else if existing. If the crosshair is unresponsive in stage selection screen, before pressing Start, try to wait 5 seconds after the demo game video is shown.

For Point Blank X, to fix the ticket dispenser error and memory test freeze, append following lines to file ".\PBX100-2-NA-MPR0-A63_Data\Setting.ini" in game folder:

TICKET 0
<br>
MAIN_PATH ./NVRAM/
<br>
BACKUP_PATH ./NVRAM/

For Haunted Museum II and Gaia Attack 4, to fix the movie read error, install [wmv9VCMsetup](https://www.videohelp.com/software/WMV9-VCM), also in Windows command prompt with admin privilege, run "regsvr32 %SystemRoot%\SysWOW64\ir50_32.dll". In game settings, uncheck Custom Crosshairs - Enable.

For games like The House of the Dead 4 without in-game crosshair, copy crosshair images P1.png and P2.png to folder of the game startup program, and check Crosshairs - Enable and Crosshairs - Scaling in game settings. But if an inactive player's crosshair is shown, try to rename the corresponding png file to something else to hide it.

For games with aspect ratio of 4:3, if your screen's resolution is 16:9, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio.

<br>

## < RPCS3 > emulator PC lightgun aiming

For PS3 games like Time Crisis: Razing Storm (Time Crisis 4 Arcade Ver, Razing Storm, Deadstorm Pirates), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In RPCS3 game's GPU configuration, set Framelimit to Auto, check Write Color Buffers (required in order to fix screen brightness), check VSync. In I/O tab, set Mouse Handler to Basic, Move Handler to Mouse, Camera Input to PS Eye, Camera Handler to Fake, check Show PS Move Cursor. In Advanced tab, set VBlank Frequency to 59 Hz, uncheck VBlank NTSC Fixup (only available in game custom configuration, and it's important in order to get correct mouse button response).

In Mice->Basic Mouse configuration, set Button 1/2/3/4/5 to Mouse Left/Right/Middle/Back/Fwd respectively, set Button 6/7/8 to 6/7/8 (without Num+) respectively. In USB Devices->PS Move (Mouse) configuration, set Start/Select/Triangle/Circle/Cross/Square/Move/T to Mouse 7/6/4/5/2/3/8/1 respectively, and clear all other buttons. In Gamepad configuration, setup a keyboard or gamepad handler for PS3 Controller to navigate menus in game, as RPCS3 doesn't support PS Move navigation. When using a keyboard handler, use Ctrl-F11 in game to switch between PS3 Controller mode and PS Move mode.

In the crosshair calibration screen, make sure PS Move mode is active. Keep in window mode and resize the window as large as possible at the center of the screen while matching the game's aspect ratio (required in order to align the Windows cursor with the PS Move cursor).

For Time Crisis 4 and Razing Storm, press Trigger to start calibration. Except the center target, you should shoot each target at a little further from the outermost ring toward the window edge to get the correct calibration. But don't shoot too far, otherwise you can't turn left/right in the game when you need to point the crosshair to the window edge. For Deadstorm Pirates, press Back button to start calibration, just shoot at the center of each target.

Press Touchpad East to retry, or press Touchpad North to confirm, then Touchpad East to go back to title screen. Press Touchpad Center to select menu items and start a new game. Make sure the player controller is set to Motion Controller No.7.

After calibration, you can uncheck Show PS Move Cursor in I/O configuration. Optionally hide the Windows cursor by [nomousy](https://www.autohotkey.com/board/topic/2083-nomousy-disablehide-your-mouse-pointer-cmd/) ([download](https://www.mediafire.com/file/oglzpabl50b8juq/nomousy.zip/file)), run "nomousy /hide" to switch the Windows cursor on/off.

<br>

## < PCSX2 > emulator PC lightgun aiming

For PS2 games.

(Option 2 works better)

### Option 1: Lightgun emulation replacing mouse (e.g. Time Crisis 3)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In PCSX2's Emulation settings, check Vertical Sync. In Graphics settings -> Display tab, check Show Overscan (better for some games). In Controller settings -> USB Port 1, select GunCon 2. In Bindings tab, set Trigger to Pointer-0 Left Button, Shoot Offscreen to Pointer-0 Right Button, Calibration Shot to Keyboard 8 (without Numpad). Set Buttons A/B/C/Start/Select to Pointer-0 Middle Button, Pointer-0 Button5, Pointer-0 Button4, Keyboard 7, Keyboard 6 respectively. Set D-Pad Up/Down/Left/Right to Keyboard Numpad8/5/4/6. In Settings tab, set a crosshair png image in Cursor Path, check Manual Screen Configuration, set X Scale to 90%, Y Scale to 97% (different for some games, if the crosshair moving scale during calibration is incorrect, try X Scale around 84% to 90%, Y Scale around 92% to 119%), Center X to 420px, leave others to default.

For games like Resident Evil: Dead Aim which require the D-pad to work, you can map the D-pad keys by assigning Numeric keypad 8/5/4/6 to Non-Press Touchpad North/South/West/East. Also change other assignments to suit the game.

If the custom crosshair image doesn't show up, it may be a bug of PCSX2. Try to modify Cursor Scale in the GunCon 2 Settings tab to fix. Press Alt-Enter to switch to fullscreen.

In the calibration screen, press Back button to start calibration, and follow the game's instructions to confirm.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Vampire Night)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Y, Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B, West: Gamepad LB, East: Gamepad RB, North: Gamepad X, South: Pointer reset

In PCSX2's Emulation settings, check Vertical Sync. In Graphics settings -> Display tab, check Show Overscan (better for some games). In Controller settings -> USB Port 1, select GunCon 2. In Bindings tab, click Automatic Mapping, select SDL-0 (XInput Controller). Press Touchpad South to reset stick, and set the mapping by pressing the buttons on Gear VR controller. Set Trigger to SDL-0 Face South, Shoot Offscreen to SDL-0 Face East, Calibration Shot to SDL-0 Face North. Set Buttons A/B/C to SDL-0 Left Shoulder, SDL-0 Right Shoulder, SDL-0 Face West respectively. Set Relative Aiming Up/Down/Left/Right to SDL-0 -Left Y/+Left Y/-Left X/+Left X. In Settings tab, set a crosshair png image in Cursor Path, uncheck Manual Screen Configuration.

Alternatively, edit the ini file "%USERPROFILE%\Documents\PCSX2\inis\PCSX2.ini" directly for the mapping:

[USB1]
<br>
Type = guncon2
<br>
guncon2_Up = SDL-0/DPadUp
<br>
guncon2_Down = SDL-0/DPadDown
<br>
guncon2_Left = SDL-0/DPadLeft
<br>
guncon2_Right = SDL-0/DPadRight
<br>
guncon2_Trigger = SDL-0/FaceSouth
<br>
guncon2_ShootOffscreen = SDL-0/FaceEast
<br>
guncon2_A = SDL-0/LeftShoulder
<br>
guncon2_B = SDL-0/RightShoulder
<br>
guncon2_C = SDL-0/FaceWest
<br>
guncon2_Select = SDL-0/Back
<br>
guncon2_Start = SDL-0/Start
<br>
guncon2_Recalibrate = SDL-0/FaceNorth
<br>
guncon2_RelativeUp = SDL-0/-LeftY
<br>
guncon2_RelativeDown = SDL-0/+LeftY
<br>
guncon2_RelativeLeft = SDL-0/-LeftX
<br>
guncon2_RelativeRight = SDL-0/+LeftX

For games like Resident Evil: Dead Aim which require the D-pad to work, you can map the D-pad buttons by assigning Gamepad D-pad Up/Down/Left/Right to Non-Press Touchpad North/South/West/East. Also change other assignments to suit the game.

If the custom crosshair image doesn't show up, it may be a bug of PCSX2. Try to modify Cursor Scale in the GunCon 2 Settings tab to fix. Press Alt-Enter to switch to fullscreen.

In the calibration screen, press Back button to start calibration, and follow the game's instructions to confirm.

<br>

## < DuckStation > emulator PC lightgun aiming

For PS1 games.

(Option 2 works better)

### Option 1: Lightgun emulation replacing mouse (e.g. Time Crisis: Project Titan)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: K (used when pressing at the same time both Buttons A and B of the gun)
<br>
Touchpad - Center: Mouse right button, West: K, East: L, North: Unassigned, South: Pointer reset

In DuckStation's Emulation settings, check Vertical Sync. In Graphics settings -> Rendering tab, set Crop to None (better for some games). In Controller settings -> Global Settings, check Enable Mouse Mapping, uncheck Use Raw Input. In Controller Port 1 page, select GunCon. In Bindings tab, click Clear Mapping. Set Fire to Pointer-0/LeftButton, Fire Offscreen to Pointer-0/RightButton. Set Side Buttons A/B to Keyboard/K, Keyboard/L respectively. In Settings tab, set X Scale to 100% (different for some games, if the crosshair moving scale during calibration is incorrect, try around 98% to 100%).

Press F11 to switch to fullscreen.

For games like Crypt Killer, select Justifier in Controller Port 1 and set the same key mapping. In Settings tab, set X Scale to 99%, Line Start Offset to -5, Tick Offset to 0, and calibrate the crosshair in game.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Point Blank 3)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad LB (used when pressing at the same time both Buttons A and B of the gun)
<br>
Touchpad - Center: Gamepad B, West: Gamepad LB, East: Gamepad RB, North: Unassigned, South: Pointer reset

In DuckStation's Emulation settings, check Vertical Sync. In Graphics settings -> Rendering tab, set Crop to None (better for some games). In Controller settings -> Controller Port 1, select GunCon. In Bindings tab, click Clear Mapping. Press Touchpad South to reset stick, and set the mapping by pressing the buttons on Gear VR controller. Set Fire to SDL-0/A, Fire Offscreen to SDL-0/B. Set Side Buttons A/B to SDL-0/LeftShoulder, SDL-0/RightShoulder respectively. Set Relative Aiming Up/Down/Left/Right to SDL-0/-LeftY, SDL-0/+LeftY, SDL-0/-LeftX, SDL-0/+LeftX respectively. In Settings tab, set X Scale to 98% (different for some games, if the crosshair moving scale during calibration is incorrect, try around 98% to 100%). If setting for 2 players, set different crosshair png images in Crosshair Image Path.

Alternatively, edit the ini file "%USERPROFILE%\Documents\DuckStation\settings.ini" directly for the mapping:

[Pad1]
<br>
Type = GunCon
<br>
Trigger = SDL-0/A
<br>
ShootOffscreen = SDL-0/B
<br>
A = SDL-0/LeftShoulder
<br>
B = SDL-0/RightShoulder
<br>
RelativeUp = SDL-0/-LeftY
<br>
RelativeDown = SDL-0/+LeftY
<br>
RelativeLeft = SDL-0/-LeftX
<br>
RelativeRight = SDL-0/+LeftX

Press F11 to switch to fullscreen.

For games like Crypt Killer, select Justifier in Controller Port 1 and set the same key mapping. In Settings tab, set X Scale to 100%, Line Start Offset to -14, Tick Offset to 50, and set Crosshair Image Path when necessary. Calibrate the crosshair in game. If editing the ini file for mapping:

[Pad1]
<br>
Type = Justifier
<br>
Trigger = SDL-0/A
<br>
ShootOffscreen = SDL-0/B
<br>
RelativeUp = SDL-0/-LeftY
<br>
RelativeDown = SDL-0/+LeftY
<br>
RelativeLeft = SDL-0/-LeftX
<br>
RelativeRight = SDL-0/+LeftX
<br>
Start = SDL-0/LeftShoulder
<br>
Back = SDL-0/RightShoulder

<br>

## < Dolphin > emulator PC lightgun aiming

For Wii games.

### Option 1: Lightgun emulation replacing mouse (e.g. Ghost Squad)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse right button, Back: Q, Home: E, +: 1, -: 2
<br>
Touchpad - Center: Mouse left button, West: Left arrow, East: Right arrow, North: Mouse middle button, South: Pointer reset

In Dolphin's Configuration -> Interface, set Mouse Cursor Visibility to Always. In Graphics settings, check V-Sync. In Controller settings, under the Wii Remotes section, select Emulate the Wii's Bluetooth adapter, set Wii Remote 1 to Emulated Wii Remote. Click Configure, set Device to DInput/0/Keyboard Mouse, then click Default. In Motion Simulation tab, under the Point section, set Vertical Offset to 15 cm, set Total Yaw to 19 degree , set Total Pitch to 19 degree (different for some games, try Total Yaw around 15 to 19 degree, and Total Pitch around 11 to 19 degree, or try to find the data in [Dolphin Lightguns Accuracy Inis](https://github.com/ProfgLX/Dolphin-Lightguns-Accuracy-Inis)). Give the Profile a name and Save, then Close the settings. Don't click Calibrate, it doesn't work.

For games like Resident Evil: The Umbrella Chronicles which use the Nunchuk stick, you can map the Nunchuk stick keys by assigning W/S/A/D to Non-Press Touchpad North/South/West/East. Also change other assignments to suit the game.

Some games use shake to reload, it's mapped to mouse middle button (Touchpad North) by default.

After starting the game, if the crosshair moving scale is incorrect, try to adjust Total Yaw or Total Pitch in Controller settings. When ready, set Mouse Cursor Visibility to Never in Interface configuration. Press Alt-Enter to switch to fullscreen.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. The House of the Dead: Overkill)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad B, Back: Gamepad Back/View, Home: Gamepad Start/Menu, +: Gamepad RB, -: Gamepad LB
<br>
Touchpad - Center: Gamepad A, West: Gamepad D-pad Left, East: Gamepad D-pad Right, North: Gamepad X, South: Pointer reset

In Dolphin's Graphics settings, check V-Sync. In Controller settings, under the Wii Remotes section, select Emulate the Wii's Bluetooth adapter, set Wii Remote 1 to Emulated Wii Remote. Click Configure, set Device to XInput/0/Gamepad. Press Touchpad South to reset stick, and set the mapping by pressing the buttons on Gear VR controller. Set Buttons A/B/1/2/-/+ to Button A, Button B, Shoulder R, Shoulder L, Back, Start respectively. Set D-Pad Left/Right to Pad W, Pad E respectively. In Motion Simulation tab, under the Shake section, set all of X/Y/Z to Button X. Under the Point section, set Up/Down/Left/Right to Left Y+, Left Y-, Left X-, Left X+ respectively. Set Vertical Offset to 15 cm, Total Yaw to 19 degree, Total Pitch to 19 degree (different for some games, usually Total Yaw around 15 to 19 degree, and Total Pitch around 11 to 19 degree, try to find the data in [Dolphin Lightguns Accuracy Inis](https://github.com/ProfgLX/Dolphin-Lightguns-Accuracy-Inis)). Give the Profile a name and Save, then Close the settings. Don't click Calibrate, it doesn't work.

Alternatively, edit the ini file "%APPDATA%\Dolphin Emulator\Config\WiimoteNew.ini" directly for the mapping:

[Wiimote1]
<br>
Device = XInput/0/Gamepad
<br>
Source = 1
<br>
Buttons/A = \`Button A\`
<br>
Buttons/B = \`Button B\`
<br>
Buttons/1 = \`Shoulder R\`
<br>
Buttons/2 = \`Shoulder L\`
<br>
Buttons/- = Back
<br>
Buttons/+ = Start
<br>
D-Pad/Up = \`Pad N\`
<br>
D-Pad/Down = \`Pad S\`
<br>
D-Pad/Left = \`Pad W\`
<br>
D-Pad/Right = \`Pad E\`
<br>
IR/Up = \`Left Y+\`
<br>
IR/Down = \`Left Y-\`
<br>
IR/Left = \`Left X-\`
<br>
IR/Right = \`Left X+\`
<br>
Shake/X = \`Button X\`
<br>
Shake/Y = \`Button X\`
<br>
Shake/Z = \`Button X\`

For games like Resident Evil: The Umbrella Chronicles which use the Nunchuk stick, you can map the Nunchuk stick directions by assigning Gamepad RS Up/Down/Left/Right to Non-Press Touchpad North/South/West/East. Then in Controller settings, set Extension to Nunchuk and in Configure Extension, set Up/Down/Left/Right to Right Y+, Right Y-, Right X-, Right X+ respectively, Save the Profile. Also change other assignments to suit the game. If editing the ini file for mapping:

[Wiimote1]
<br>
Extension = Nunchuk
<br>
Nunchuk/Stick/Up = \`Right Y+\`
<br>
Nunchuk/Stick/Down = \`Right Y-\`
<br>
Nunchuk/Stick/Left = \`Right X-\`
<br>
Nunchuk/Stick/Right = \`Right X+\`

Some games use shake to reload, it's mapped to Gamepad X (Touchpad North).

Press Alt-Enter to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio.

<br>

## < Snes9x > emulator PC lightgun aiming

For SNES games like Yoshi's Safari, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Home: /? (default for Pause)
<br>
Touchpad - Center: Mouse right button, North: `~ (default for Turbo), South: Pointer reset

In Snes9x's Video menu -> Display Configuration, check VSync. In Input menu, select Use Super Scope.

After starting the game, press Alt-Enter to switch to fullscreen. Adjust the gun crosshair in game when necessary.

<br>

## < FCEUX > emulator PC lightgun aiming

For NES games like Duck Hunt, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: S (default for Select), Home: Enter (default for Start)
<br>
Touchpad - Center: Mouse right button, South: Pointer reset

In FCEUX's GUI config, uncheck Enable right-click context menu. In Video config, under Full Screen Settings, check Hide mouse cursor, set Sync method to Wait for VBlank. In Input config, set Port 1 to Gamepad and use your preferred configuration by keyboard or a physical gamepad, set Port 2 to Zapper. If you use keyboard default mapping for gamepad, Enter of Start button will conflict with Alt-Enter of toggling fullscreen. Fix it by going to Map Hotkeys config, setting Toggle Fullscreen to F11.

After starting the game, switch to fullscreen. If the resolution is incorrect, you need to set in the fceux64.exe Compatibility properties, click Change high DPI settings, check Override high DPI scaling behavior, set Scaling performed by: to Application, and restart FCEUX.

<br>

## < Flycast > emulator PC lightgun aiming

For Dreamcast games like Confidential Mission.

### Option 1: Lightgun emulation replacing mouse

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Home: Mouse middle button (default for Start), +: Up arrow, -: Down arrow
<br>
Touchpad - Center: Mouse X1 button, West: Left arrow, East: Right arrow, North: Mouse right button (default for B), South: Pointer reset

In Flycast's Video settings, check VSync. In Controls settings, for Default Mouse, select Port A, click Map, select Dreamcast Controls, Reset the mapping. Then map Reload to Button 4, click Done. For Keyboard, select Port A, click Map, Reset the mapping, click Done. Under Dreamcast Devices, set Port A to Light Gun, select Sega VMU, check Crosshair. To hide the crosshair of inactive player, set the corresponding crosshair color alpha value (A) to 0.

Press F11 to switch to fullscreen. Calibrate the gun crosshair in game's Options menu.

For Naomi and Atomiswave arcade games (e.g. Ninja Assault), in General settings, uncheck Hide Legacy Naomi Roms, set the mapping for Keyboard and Default Mouse by selecting Arcade Controls in the mapping screens (in service menu of some games, Button 3 corresponds to ENTER SW, Up/Down for navigation). Calibrate the gun crosshair in the game's Service and Test menu.

### Option 2: Lightgun emulation replacing gamepad left stick

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Home: Gamepad Start/Menu, +: Gamepad D-pad Up, -: Gamepad D-pad Down
<br>
Touchpad - Center: Gamepad X, West: Gamepad D-pad Left, East: Gamepad D-pad Right, North: Gamepad B, South: Pointer reset

In Flycast's Video settings, check VSync. In Controls settings, for Xbox 360 Controller, select Port A, click Map, select Dreamcast Controls, Reset the mapping. Press Touchpad South to reset stick, and set the mapping by pressing the buttons on Gear VR controller. Set Reload by pressing Touchpad Center. Under Dreamcast Devices, set Port A to Light Gun, select Sega VMU, check Crosshair. To hide the crosshair of inactive player, set the corresponding crosshair color alpha value (A) to 0.

Press F11 to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio. Calibrate the gun crosshair in game's Options menu.

For Naomi and Atomiswave arcade games (e.g. Ninja Assault), in General settings, uncheck Hide Legacy Naomi Roms, set the mapping for Xbox 360 Controller by selecting Arcade Controls in the mapping screen (in service menu of some games, Button 3 corresponds to ENTER SW, Up/Down for navigation). Calibrate the gun crosshair in the game's Service and Test menu.

<br>

## < Supermodel > emulator PC lightgun aiming

For Model 3 arcade games like The Lost World: Jurassic Park.

### Option 1: Lightgun emulation replacing mouse

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 3, Touchpad Center: Mouse right button, Touchpad South: Pointer reset

In Supermodel's Core settings, set InputSystem to dinput. In Video settings, check FullScreen (required in order to hide cursor), check VSync, check NoWhiteFlash, set Crosshairs to 1.

Calibrate the gun crosshair in the game's Service and Test menu. If unable to exit the calibration screen by pressing 7 (default for Test), try to press 5 (default for Service) and 7 together several times.

### Option 2: Lightgun emulation replacing gamepad left stick

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad LS Button (default for Start), Home: Gamepad RS Button (default for Coin)
<br>
Touchpad Center: Gamepad B, Touchpad South: Pointer reset

In Supermodel's Core settings, set InputSystem to dinput. In Video settings, check FullScreen (required in order to hide cursor), check VSync, check NoWhiteFlash, set Crosshairs to 1 (1: player 1 only, 2: player 2 only, 3: both players).

By default, only player 1 gun is mapped to gamepad, if you want to map player 2 gun to second gamepad, you need to edit the ini file .\Config\Supermodel.ini in Supermodel folder:

InputAnalogGunX2 = JOY2_XAXIS
<br>
InputAnalogGunY2 = JOY2_YAXIS
<br>
InputAnalogTriggerLeft2 = JOY2_BUTTON1
<br>
InputAnalogTriggerRight2 = JOY2_BUTTON2

Supermodel has a little dead zone for gamepad by default, you can set the dead zone to 0 by appending the following lines to the ini file (edit if existing):

InputJoy1XDeadZone = 0
<br>
InputJoy1YDeadZone = 0
<br>
InputJoy2XDeadZone = 0
<br>
InputJoy2YDeadZone = 0

After starting the game, don't move the mouse, otherwise input will be switched to mouse automatically by default. Optionally, you can remove the mouse mapping from InputAnalogGunX/Y in the ini file. 

If your screen's resolution is 16:9 and the game is 4:3, set motion pointer AR correction to 1333 in app to get the correct crosshair moving aspect ratio.

Calibrate the gun crosshair in the game's Service and Test menu. If unable to exit the calibration screen by pressing 7 (default for Test), try to press 5 (default for Service) and 7 together several times.

<br>

## < Demul > emulator PC lightgun aiming

For Hikaru arcade games like Brave Firefighters, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: 1, Home: 5
<br>
Touchpad - Center: Gamepad B, North: Gamepad X, South: Pointer reset

In Demul's Video config, check Vsync. In Maple Device Manager config, set PORT C to Lightgun.

The game uses a curved crosshair movement which makes aiming distorted. To get the correct light gun aiming, download [DemulShooter](https://github.com/argonlefou/DemulShooter/releases), run DemulShooter_GUI, in Page Selection, select P1 Configuration, set P1 Device to [Gamepad] [Unknown Manufacturer] - Controller (XBOX 360 For Windows), Save Config. In Windows command prompt with admin privilege, run "DemulShooter -target=demul07a -rom=braveff".

After starting game, press F4 to enter Service and Test menu, F4 again to exit (required in order to turn on audio).

Press Alt-Enter to switch to fullscreen. If the resolution is incorrect, you need to set in the demul.exe Compatibility properties, click Change high DPI settings, check Override high DPI scaling behavior, set Scaling performed by: to Application, and restart Demul.

Optionally, if your screen isn't 4:3 and you want to play the game in 4:3, download [NirCmd 64-bit](https://www.nirsoft.net/utils/nircmd.html), run "nircmd win -style process demul.exe 0xC00000" to hide title bar and "nircmd win setsize process demul.exe 240 0 1440 1080" (example of 1920x1080 screen, change numbers to suit your screen's resolution) to switch to maximized window.

Calibrate the crosshair in the game's Service and Test menu -> B.F.F. TEST MENU -> NOZZLE SENSOR SETTING. Press Touchpad South to reset stick, to get a better calibration, during "Aim at CENTER of the screen", press Trigger when CC X:7f Y:7f is shown. Alternatively, calibration can be done easily by mouse without running DemulShooter.

<br>

## Backup of user config

You can back up the user config file for different settings or game profiles. Exit the app first and it's inside a sub-sub folder in %LOCALAPPDATA%\Gear_VR_Controller

<br>

## Hints on low input lag for games and emulators

- Turn on game mode of TV or monitor if available
- Turn on low latency mode or anti-lag of GPU driver
- Keep the controller within good coverage of Bluetooth
