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
- No pairing needed, just turn on PC Bluetooth and install batteries to the controller
- Press any button on the controller, then click the Search icon in app
- Click the Connect button, that's it

Calibration for motion sensing and motion pointer
- Place the controller upside down on a stable surface, then click the CAL button, that's it

Download latest version

- v2.1.12 (from [Softpedia](https://www.softpedia.com/get/System/System-Miscellaneous/Gear-VR-Controller.shtml))
- md5: c080da6b865b3299b0341e5384e12df2
- sha-1: a2aa53c1004980fda0742bfc3368f0505ddb54df

System requirements
- Windows 10 x64 or Windows 11
- [.NET Desktop Runtime 9.0](https://dotnet.microsoft.com/download/dotnet/9.0)

[Major change log](https://github.com/ShimuraWorkshop/Gear-VR-Controller-Motion-Pointer-for-Windows/wiki#major-change-log)

[Troubleshooting](https://github.com/ShimuraWorkshop/Gear-VR-Controller-Motion-Pointer-for-Windows/wiki#troubleshooting)

<br>

Details
- [\*Secret\* gyro/motion gamepad emulation](#secret-gyromotion-gamepad-emulation-in-new-version)
- [Lightgun emulation](#lightgun-emulation)
- [< The House of the Dead 2: Remake > PC gyro aiming](#-the-house-of-the-dead-2-remake--pc-gyro-aiming-sample-config)
- [< The House of the Dead: Remake > PC gyro/lightgun aiming](#-the-house-of-the-dead-remake--pc-gyrolightgun-aiming-sample-config)
- [< Panzer Dragoon: Remake > PC gyro aiming](#-panzer-dragoon-remake--pc-gyro-aiming-sample-config)
- [< Blue Estate The Game > PC lightgun aiming](#-blue-estate-the-game--pc-lightgun-aiming-sample-config)
- [< The Typing of the Dead: Overkill > PC lightgun aiming](#-the-typing-of-the-dead-overkill--pc-lightgun-aiming-sample-config)
- [< The House of the Dead III > PC lightgun aiming](#-the-house-of-the-dead-iii--pc-lightgun-aiming-sample-config)
- [< The House of the Dead 2 > PC lightgun aiming](#-the-house-of-the-dead-2--pc-lightgun-aiming-sample-config)
- [< House of the Dead: Scarlet Dawn > PC lightgun aiming](#-house-of-the-dead-scarlet-dawn--pc-lightgun-aiming-sample-config)
- [< MAME > emulator PC lightgun aiming (for Virtua Cop, Time Crisis, Alien 3: The Gun, etc)](#-mame--emulator-pc-lightgun-aiming-sample-config)
- [< Cxbx-Reloaded > emulator PC lightgun aiming (for Virtua Cop 3, Silent Scope 2)](#-cxbx-reloaded--emulator-pc-lightgun-aiming-sample-config)
- [< TeknoParrot > emulator PC lightgun aiming (for Time Crisis 5, Operation GHOST, etc)](#-teknoparrot--emulator-pc-lightgun-aiming-sample-config)
- [< RPCS3 > emulator PC lightgun aiming (for Time Crisis: Razing Storm, etc)](#-rpcs3--emulator-pc-lightgun-aiming-sample-config)
- [< PCSX2 > emulator PC lightgun aiming (for Time Crisis 3, Vampire Night, etc)](#-pcsx2--emulator-pc-lightgun-aiming-sample-config)
- [< DuckStation > emulator PC lightgun aiming (for Time Crisis: Project Titan, Point Blank 3, etc)](#-duckstation--emulator-pc-lightgun-aiming-sample-config)
- [< Dolphin > emulator PC lightgun aiming (for Ghost Squad, etc)](#-dolphin--emulator-pc-lightgun-aiming-sample-config)
- [< Snes9x > emulator PC lightgun aiming (for Yoshi's Safari, etc)](#-snes9x--emulator-pc-lightgun-aiming-sample-config)
- [< FCEUX > emulator PC lightgun aiming (for Duck Hunt, etc)](#-fceux--emulator-pc-lightgun-aiming-sample-config)
- [< Flycast > emulator PC lightgun aiming (for Confidential Mission, Ninja Assault, etc)](#-flycast--emulator-pc-lightgun-aiming-sample-config)
- [< Supermodel > emulator PC lightgun aiming (for The Lost World: Jurassic Park, etc)](#-supermodel--emulator-pc-lightgun-aiming-sample-config)
- [< Demul > emulator PC lightgun aiming (for Brave Firefighters, etc)](#-demul--emulator-pc-lightgun-aiming-sample-config)
- [Backup of user config](#backup-of-user-config)
- [Hints on low input lag](#hints-on-low-input-lag-for-games-and-emulators)

<br>

Gear VR is a trademark or registered trademark of Samsung Electronics Co., Ltd.
<br>
​Windows is a trademark or registered trademark of Microsoft Corporation

<br>

## \*Secret\* gyro/motion gamepad emulation in new version

Now you can use the controller like a gyro gamepad. Gyro aiming together with analog touch stick (needn't press) are supported. Gamepad buttons and sticks are added to key assignment list for mapping to touchpad press (8 directions, center and lower edge), other 5 buttons and 12 motions.

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

Adjust the motion pointer speed to around 1~4 in app and switch to motion pointer mode before starting game. Also adjust the cursor speed in Windows mouse settings when necessary. For easier control, assign "Toggle between cursor and pointer mode" or "Pointer temporary off" to a button, or assign "Pointer temporary on" to the new second action of buttons by modifying any of these options:

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

ViGEmBus not required, update the app to v2.1.12, extract the config to "C:\Program Files\Gear VR Controller" (default).

Assign "Pointer reset" to Touchpad South, "Mouse left button" to Trigger, also other keys to suit the game. Adjust the motion pointer speed to around 8~12 in app and switch to motion pointer mode before starting game.

### Option 2: Lightgun emulation replacing gamepad stick

Config file [Link](https://www.mediafire.com/file/lo7iu6lflxh00hl/Gear_VR_Controller.dll.config_lightgun.by.gamepad.zip/file) (if supported by the game or emulator)

Install [ViGEmBus](https://github.com/nefarius/ViGEmBus/releases/tag/v1.22.0), update the app to v2.1.12, extract the config to "C:\Program Files\Gear VR Controller" (default).

Assign "Pointer reset" to Touchpad South, "Gamepad A" to Trigger, also other keys to suit the game. Adjust the motion pointer speed to around 8~12 in app for the game.

With either config, if the game or emulator is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

<br>

## < The House of the Dead 2: Remake > PC gyro aiming sample config

Config file
[Link](https://www.mediafire.com/file/ca3mrdhr4q8jl0g/Gear_VR_Controller.dll.config_the.house.of.the.dead.2.remake.zip/file)

ViGEmBus not required, update the app to v2.1.12, extract the config to "C:\Program Files\Gear VR Controller\" (default), then assign keys for example:

Trigger: Mouse left button, Back: Enter, Home: Tab, +: F, -: Esc
<br>
Touchpad - Center: Mouse right button, West: Q, East: E, South: Pointer temporary off, North: Unassigned

Touchpad (without press) is mapped to WASD by default, you can change it by modifying KeyTouchDirectNorth/East/South/West/Center in the config file (and restarting app, text editor needs to be run as admin) when necessary.

Adjust the motion pointer speed to around 4 in app and switch to motion pointer mode before starting the game. Also adjust the cursor speed in Windows mouse settings when necessary. In game options, set controller to Keyboard/Mouse, aiming stick to Both Sticks, mouse sensitivity to 1.0, crosshair speed to 1.0.

<br>

## < The House of the Dead: Remake > PC gyro/lightgun aiming sample config

Config file for gyro aiming
[Link](https://www.mediafire.com/file/yxi0v4sfd9ypkyy/Gear_VR_Controller.dll.config_the.house.of.the.dead.remake.zip/file)

ViGEmBus not required, update the app to v2.1.12, extract the config to "C:\Program Files\Gear VR Controller\" (default), adjust the motion pointer speed to around 4 in app, and also adjust the cursor speed in Windows mouse settings when necessary. Then assign keys for example:

Trigger: Mouse left button, Back: Enter, -: Esc
<br>
Touchpad - Center: Mouse right button, West: Q, East: E, North: F, South: Pointer temporary off

If you have installed a lightgun or arcade plugin (like [this](https://steamcommunity.com/app/1694600/discussions/0/3271312219438716734/) or [this](https://github.com/argonlefou/HotdRemake_ArcadePlugin/)), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and change the key assignments according to the plugin.

With either config, switch to motion pointer mode before starting the game, then in game options, set controller type to Keyboard/Mouse, sensitivity to 1.0, crosshair speed to 1.00 (some settings may be unavailable in arcade plugin).

<br>

## < Panzer Dragoon: Remake > PC gyro aiming sample config

Use the same config file as < The House of the Dead 2: Remake >, and change the key assignments to match the game. But the game has forced mouse smoothing, you need to move the controller slowly.

<br>

## < Blue Estate The Game > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game. In game's Controls settings, switch controller to Mouse, set Mouse in Raw Mode to Yes, Gestures with the Mouse to Yes.

<br>

## < The Typing of the Dead: Overkill > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game.

<br>

## < The House of the Dead III > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game.

<br>

## < The House of the Dead 2 > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys to suit the game. In game's config, select Mouse + Keyboard for player controller.

<br>

## < House of the Dead: Scarlet Dawn > PC lightgun aiming sample config

For TeknoParrot, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Back/View
<br>
Touchpad - West: Gamepad LB, North: Gamepad X, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to XInput, uncheck General - Windowed, check General - HideCursor, check Crosshairs - Enable Native. In controller setup, set the mapping by pressing the buttons on Gear VR controller. For easier input during setup, set motion pointer speed to 1 and dead zone to 10000 in app, then for Player 1, set Start by pressing Back, Gun Trigger by Trigger, Sub Trigger by Touchpad North, Controller Select by Touchpad West. Set dead zone back to 15 (default) and press Touchpad South to reset stick, then set Player 1 Gun X by pointing the controller rightward slowly until X+ is shown, set Gun Y by pointing upward until Y+ is shown.

Adjust the motion pointer speed to around 8~12 for the game.

<br>

## < MAME > emulator PC lightgun aiming sample config

### Option 1: Lightgun emulation replacing mouse (e.g. Time Crisis, Virtua Cop)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 5
<br>
Touchpad - Center: Mouse right button, North: Mouse middle button, South: Pointer reset

In MAME game's Input Device Options, set Lightgun Device Assignment to lightgun, Pedal Device Assignment to lightgun, Keyboard Input Provider to dinput, Lightgun Input Provider to win32.

Keep in maximized window mode or press Alt-Enter to switch to fullscreen. But in fullscreen mode, if your screen's resolution is 16:9 and the game is 4:3, you need to modify ScalePointerX from 1000 to 1333 in the config file in order to get the correct crosshair moving scale (and restart app, text editor needs to be run as admin).

If you want to use non-press Touchpad for pedal, modify KeyTouchDirectCenter from Unassigned to Mouse right button in the config file.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Alien 3: The Gun)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: 1, Home: 5
<br>
Touchpad - Center: Gamepad B, North: Gamepad X, South: Pointer reset

Press Touchpad South to reset stick. In MAME game's Input Device Options, set Keyboard Input Provider to dinput, Joystick Input Provider to xinput. In Advanced Options, set Joystick to On, Joystick deadzone to 0, Joystick saturation to 1.

Press Alt-Enter to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, you need to modify ScaleYaw from 1000 to 1333 in the config file in order to get the correct crosshair moving scale (and restart app, text editor needs to be run as admin).

For some games like Terminator 2: Judgment Day which need to calibrate the gun for player 2, if not playing, press keyboard key A (default for player 2's gun trigger) to pass.

With either config, press Tab, select Crosshair Options, set Visibility to Always or Never when necessary (maybe unavailable in some games). Calibrate the gun crosshair in the game's Service and Test menu.

<br>

## < Cxbx-Reloaded > emulator PC lightgun aiming sample config

For Virtua Cop 3, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad B (for Reload during ES Mode), Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B (for Reload), West: Gamepad X (for Weapon Change), North: Gamepad LT (for ES Mode), South: Pointer reset

In Cxbx-Reloaded's Input settings, select MS Gamepad S, click Configure, set Device to XInput/0/Gamepad, click Default Bindings, then give the Profile a name and Save. In Video settings, set Display Resolution to your screen resolution and refresh rate, uncheck Use Exclusive Fullscreen Mode, check Maintain Aspect Ratio, and check Force VSync. Delete the file boot.id in the root folder of game if existing.

Open the game by vc3.xbe, start emulation. Press Alt-Enter to switch to fullscreen. As the game is 4:3, if your screen's resolution is 16:9, you need to modify ScaleYaw from 1000 to 1333 in the config file in order to get the correct crosshair moving scale (and restart app, text editor needs to be run as admin). Due to the curved crosshair movement used by the game, aim will have some distortions especially at corners of the screen.

For Silent Scope 2 (in Silent Scope Complete), select EMS TopGun II in Input settings, use Default Bindings. Assign Gamepad RS Button to a button/motion to hide Laser dot in game, also assign Gamepad D-pad Up/Down/Left/Right to buttons/motions for menu navigation when necessary.

<br>

## < TeknoParrot > emulator PC lightgun aiming sample config

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

For Haunted Museum II, to fix the movie read error, install [wmv9VCMsetup](https://www.videohelp.com/software/WMV9-VCM), also in Windows command prompt with admin privilege, run "regsvr32 %SystemRoot%\SysWOW64\ir50_32.dll". In game settings, uncheck Custom Crosshairs - Enable.

For games like The House of the Dead 4 without in-game crosshair, copy crosshair images P1.png and P2.png to folder of the game startup program, and check Crosshairs - Enable and Crosshairs - Scaling in game settings. But if the player 2 crosshair is shown even when not playing, rename P2.png to something else to hide it.

For games with aspect ratio of 4:3, if your screen's resolution is 16:9, you need to modify ScaleYaw from 1000 to 1333 in the config file in order to get the correct crosshair moving scale (and restart app, text editor needs to be run as admin).

<br>

## < RPCS3 > emulator PC lightgun aiming sample config

For PS3 games like Time Crisis: Razing Storm (Time Crisis 4 Arcade Ver, Razing Storm, Deadstorm Pirates), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In RPCS3 game's GPU configuration, set Framelimit to Auto, check Write Color Buffers (required in order to fix screen brightness), check VSync. In I/O tab, set Mouse Handler to Basic, Move Handler to Mouse, Camera Input to PS Eye, Camera Handler to Fake, check Show PS Move Cursor. In Advanced tab, set VBlank Frequency to 59 Hz, uncheck VBlank NTSC Fixup (only available in game custom configuration, and it's important in order to get correct mouse button response).

In Mice->Basic Mouse configuration, set Button 1/2/3/4/5 to Mouse Left/Right/Middle/Back/Fwd respectively, set Button 6/7/8 to 6/7/8 (without Num+) respectively. In USB Devices->PS Move (Mouse) configuration, set Start/Select/Triangle/Circle/Cross/Square/Move/T to Mouse 7/6/4/5/2/3/8/1 respectively, and clear all other buttons. In Gamepad configuration, setup a keyboard or gamepad handler for PS3 Controller in order to navigate menus in game, as RPCS3 doesn't support PS Move navigation. When using a keyboard handler, use Ctrl-F11 in game to switch between PS3 Controller mode and PS Move mode.

In the crosshair calibration screen, make sure PS Move mode is active. Keep in window mode and resize the window as large as possible at the center of the screen while matching the game's aspect ratio (required in order to align the Windows cursor with the PS Move cursor).

For Time Crisis 4 and Razing Storm, press Trigger to start calibration. Except the center target, you should shoot each target at a little further from the outermost ring toward the window edge to get the correct calibration. But don't shoot too far, otherwise you can't turn left/right in the game when you need to point the crosshair to the window edge. For Deadstorm Pirates, press Back button to start calibration, just shoot at the center of each target.

Press Touchpad East to retry, or press Touchpad North to confirm, then Touchpad East to go back to title screen. Press Touchpad Center to select menu items and start a new game. Make sure the player controller is set to Motion Controller No.7.

After calibration, you can uncheck Show PS Move Cursor in I/O configuration. Optionally hide the Windows cursor by [nomousy](https://www.autohotkey.com/board/topic/2083-nomousy-disablehide-your-mouse-pointer-cmd/) ([download](https://www.mediafire.com/file/oglzpabl50b8juq/nomousy.zip/file)), run "nomousy /hide" to switch the Windows cursor on/off.

<br>

## < PCSX2 > emulator PC lightgun aiming sample config

For PS2 games.

(Option 2 works better)

### Option 1: Lightgun emulation replacing mouse (e.g. Time Crisis 3)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In PCSX2's Emulation settings, check Vertical Sync. In Graphics settings -> Display tab, check Show Overscan (better for some games). In Controller settings -> USB Port 1, select GunCon 2. In Bindings tab, set Trigger to Pointer-0 Left Button, Shoot Offscreen to Pointer-0 Right Button, Calibration Shot to Keyboard 8 (without Numpad). Set Buttons A/B/C/Start/Select to Pointer-0 Middle Button, Pointer-0 Button5, Pointer-0 Button4, Keyboard 7, Keyboard 6 respectively. Set D-Pad Up/Down/Left/Right to Keyboard Numpad8/5/4/6. In Settings tab, set a crosshair png image in Cursor Path, check Manual Screen Configuration, set X Scale to 90%, Y Scale to 97% (different for some games, if the crosshair moving scale during calibration is incorrect, try X Scale around 84% to 90%, Y Scale around 92% to 119%), Center X to 420px, leave others to default.

For games like Resident Evil: Dead Aim which require the D-pad to work, you can map non-press Touchpad to D-pad keys by modifying KeyTouchDirectNorth/South/West/East from Unassigned to Numeric keypad 8/5/4/6 in the config file (and restarting app, text editor needs to be run as admin). Also change other assignments to suit the game.

If the custom crosshair image doesn't show up, it may be a bug of PCSX2. Try to modify Cursor Scale in the GunCon 2 Settings tab to fix. Press Alt-Enter to switch to fullscreen.

In the calibration screen, press Back button to start calibration, and follow the game's instructions to confirm.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Vampire Night)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Y, Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B, West: Gamepad LB, East: Gamepad RB, North: Gamepad X, South: Pointer reset

In PCSX2's Emulation settings, check Vertical Sync. In Graphics settings -> Display tab, check Show Overscan (better for some games). In Controller settings -> USB Port 1, select GunCon 2. In Bindings tab, click Automatic Mapping, select SDL-0 (XInput Controller). Then set Trigger to SDL-0 Face South, Shoot Offscreen to SDL-0 Face East, Calibration Shot to SDL-0 Face North. Set Buttons A/B/C to SDL-0 Left Shoulder, SDL-0 Right Shoulder, SDL-0 Face West respectively. Set Relative Aiming Up/Down/Left/Right to SDL-0 -Left Y/+Left Y/-Left X/+Left X. In Settings tab, click Restore Default Settings, then set a crosshair png image in Cursor Path.

For games like Resident Evil: Dead Aim which require the D-pad to work, you can map non-press Touchpad to D-pad buttons by modifying KeyTouchDirectNorth/South/West/East from Unassigned to Gamepad D-pad Up/Down/Left/Right in the config file (and restarting app, text editor needs to be run as admin). Also change other assignments to suit the game.

If the custom crosshair image doesn't show up, it may be a bug of PCSX2. Try to modify Cursor Scale in the GunCon 2 Settings tab to fix. Press Alt-Enter to switch to fullscreen.

In the calibration screen, press Back button to start calibration, and follow the game's instructions to confirm.

<br>

## < DuckStation > emulator PC lightgun aiming sample config

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

In DuckStation's Emulation settings, check Vertical Sync. In Graphics settings -> Rendering tab, set Crop to None (better for some games). In Controller settings -> Controller Port 1, select GunCon. In Bindings tab, click Clear Mapping. Set Fire to SDL-0/A, Fire Offscreen to SDL-0/B. Set Side Buttons A/B to SDL-0/LeftShoulder, SDL-0/RightShoulder respectively. Set Relative Aiming Up/Down/Left/Right to SDL-0/-LeftY, SDL-0/+LeftY, SDL-0/-LeftX, SDL-0/+LeftX respectively. In Settings tab, click Restore Default Settings. If setting for 2 players, set different crosshair png images in Crosshair Image Path.

Press F11 to switch to fullscreen.

For games like Crypt Killer, select Justifier in Controller Port 1 and set the same key mapping. In Settings tab, click Restore Default Settings, set Crosshair Image Path when necessary. Calibrate the crosshair in game.

<br>

## < Dolphin > emulator PC lightgun aiming sample config

For Wii games.

### Option 1: Lightgun emulation replacing mouse (e.g. Ghost Squad)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse right button, Back: Q, Home: E, +: 1, -: 2
<br>
Touchpad - Center: Mouse left button, West: Left arrow, East: Right arrow, North: Mouse middle button, South: Pointer reset

In Dolphin's Configuration -> Interface, set Mouse Cursor Visibility to Always. In Graphics settings, check V-Sync. In Controller settings, under the Wii Remotes section, select Emulate the Wii's Bluetooth adapter, set Wii Remote 1 to Emulated Wii Remote. Click Configure, set Device to DInput/0/Keyboard Mouse, then click Default. In Motion Simulation tab, under the Point section, set Vertical Offset to 15 cm, set Total Yaw to 19 degree (different for some games, try around 15 to 19 degree), set Total Pitch to 19 degree (different for some games, try around 11 to 19 degree). Give the Profile a name and Save, then Close the settings. Don't click Calibrate, it doesn't work.

For games like Resident Evil: The Umbrella Chronicles which use the Nunchuk stick, you can map non-press Touchpad to Nunchuk stick keys by modifying KeyTouchDirectNorth/South/West/East from Unassigned to W/S/A/D in the config file (and restarting app, text editor needs to be run as admin). Also change other assignments to suit the game.

Some games use shake to reload, it's mapped to mouse middle button (Touchpad North) by default.

After starting the game, if the crosshair moving scale is incorrect, try to adjust Total Yaw or Total Pitch in Controller settings. When ready, set Mouse Cursor Visibility to Never in Interface configuration. Press Alt-Enter to switch to fullscreen.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Ghost Squad)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad B, Back: Gamepad Back/View, Home: Gamepad Start/Menu, +: Gamepad RB, -: Gamepad LB
<br>
Touchpad - Center: Gamepad A, West: Gamepad D-pad Left, East: Gamepad D-pad Right, North: Gamepad X, South: Pointer reset

In Dolphin's Graphics settings, check V-Sync. In Controller settings, under the Wii Remotes section, select Emulate the Wii's Bluetooth adapter, set Wii Remote 1 to Emulated Wii Remote. Click Configure, set Device to XInput/0/Gamepad. Set Buttons A/B/1/2/-/+ to Button A, Button B, Shoulder R, Shoulder L, Back, Start respectively. Set D-Pad Left/Right to Pad W, Pad E respectively. In Motion Simulation tab, under the Shake section, set all of X/Y/Z to Button X. Under the Point section, set Up/Down/Left/Right to Left Y+, Left Y-, Left X-, Left X+ respectively. Set Vertical Offset to 15 cm, set Total Yaw to 19 degree (different for some games, try around 15 to 19 degree), set Total Pitch to 19 degree (different for some games, try around 11 to 19 degree). Give the Profile a name and Save, then Close the settings. Don't click Calibrate, it doesn't work.

Press Alt-Enter to switch to fullscreen. If your screen's resolution is 16:9 and the game is 4:3, you need to modify ScaleYaw from 1000 to 1333 in the config file in order to get the correct crosshair moving scale (and restart app, text editor needs to be run as admin).

For games like Resident Evil: The Umbrella Chronicles which use the Nunchuk stick, you can map non-press Touchpad to Nunchuk stick directions by modifying KeyTouchDirectNorth/South/West/East from Unassigned to Gamepad RS Up/Down/Left/Right in the config file (and restarting app, text editor needs to be run as admin). Then in Controller settings, set Extension to Nunchuk and in Configure Extension, set Up/Down/Left/Right to Right Y+, Right Y-, Right X-, Right X+ respectively, Save the Profile. Also change other assignments to suit the game.

Some games use shake to reload, it's mapped to Gamepad X (Touchpad North).

After starting the game, if the crosshair moving scale is incorrect, try to adjust Total Yaw or Total Pitch in Controller settings.

<br>

## < Snes9x > emulator PC lightgun aiming sample config

For SNES games like Yoshi's Safari, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Home: /? (default for Pause)
<br>
Touchpad - Center: Mouse right button, North: `~ (default for Turbo), South: Pointer reset

In Snes9x's Video menu -> Display Configuration, check VSync. In Input menu, select Use Super Scope.

After starting the game, press Alt-Enter to switch to fullscreen. Adjust the gun crosshair in game when necessary.

<br>

## < FCEUX > emulator PC lightgun aiming sample config

For NES games like Duck Hunt, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: S (default for Select), Home: Enter (default for Start)
<br>
Touchpad - Center: Mouse right button, South: Pointer reset

In FCEUX's GUI config, uncheck Enable right-click context menu. In Video config, under Full Screen Settings, check Hide mouse cursor, set Sync method to Wait for VBlank. In Input config, set Port 1 to Gamepad and use your preferred configuration by keyboard or a physical gamepad, set Port 2 to Zapper. If you use keyboard default mapping for gamepad, Enter of Start button will conflict with Alt-Enter of toggling fullscreen. Fix it by going to Map Hotkeys config, setting Toggle Fullscreen to F11.

After starting the game, switch to fullscreen. If the resolution is incorrect, you need to set in the fceux64.exe Compatibility properties, click Change high DPI settings, check Override high DPI scaling behavior, set Scaling performed by: to Application, and restart FCEUX.

<br>

## < Flycast > emulator PC lightgun aiming sample config

For Dreamcast games like Confidential Mission, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Home: Mouse middle button (default for Start), +: Up arrow, -: Down arrow
<br>
Touchpad - Center: Mouse X1 button, West: Left arrow, East: Right arrow, North: Mouse right button (default for B), South: Pointer reset

In Flycast's Video settings, check VSync. In Controls settings, for Default Mouse, select Port A, click Map, select Dreamcast Controls, Reset the mapping, then map Reload to Button 4, click Done. For Keyboard, select Port A, click Map, Reset the mapping, click Done. Under Dreamcast Devices, set Port A to Light Gun, select Sega VMU, check Crosshair.

After starting the game, press F11 to switch to fullscreen. Calibrate the gun crosshair in game's Options menu.

For Naomi and Atomiswave arcade games (e.g. Ninja Assault), in General settings, uncheck Hide Legacy Naomi Roms, set the mapping for Keyboard and Default Mouse by selecting Arcade Controls in the mapping screens (in service menu of some games, Button 3 corresponds to ENTER SW, Up/Down for navigation). Calibrate the gun crosshair in the game's Service and Test menu.

<br>

## < Supermodel > emulator PC lightgun aiming sample config

For Model 3 arcade games like The Lost World: Jurassic Park, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 3, Touchpad Center: Mouse right button, Touchpad South: Pointer reset

In Supermodel's Core settings, set InputSystem to dinput. In Video settings, check FullScreen (required in order to hide cursor), check VSync, set Crosshairs to 1.

Calibrate the gun crosshair in the game's Service and Test menu. If unable to exit the calibration screen by pressing 7 (default for Test), try to press 5 (default for Service) and 7 together several times.

<br>

## < Demul > emulator PC lightgun aiming sample config

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

