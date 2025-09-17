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
- [< The Typing of the Dead: Overkill > PC lightgun aiming](#-the-typing-of-the-dead-overkill--pc-lightgun-aiming-sample-config)
- [< The House of the Dead III > PC lightgun aiming](#-the-house-of-the-dead-iii--pc-lightgun-aiming-sample-config)
- [< The House of the Dead 2 > PC lightgun aiming](#-the-house-of-the-dead-2--pc-lightgun-aiming-sample-config)
- [< House of the Dead: Scarlet Dawn > PC lightgun aiming](#-house-of-the-dead-scarlet-dawn--pc-lightgun-aiming-sample-config)
- [< MAME > emulator PC lightgun aiming (for Virtua Cop, Time Crisis, etc)](#-mame--emulator-pc-lightgun-aiming-sample-config)
- [< Cxbx-Reloaded > emulator PC lightgun aiming (for Virtua Cop 3, etc)](#-cxbx-reloaded--emulator-pc-lightgun-aiming-sample-config)
- [< TeknoParrot > emulator PC lightgun aiming (for Time Crisis 5, Operation GHOST, etc)](#-teknoparrot--emulator-pc-lightgun-aiming-sample-config)
- [< RPCS3 > emulator PC lightgun aiming (for Time Crisis: Razing Storm, etc)](#-rpcs3--emulator-pc-lightgun-aiming-sample-config)
- [< PCSX2 > emulator PC lightgun aiming (for Time Crisis 3, etc)](#-pcsx2--emulator-pc-lightgun-aiming-sample-config)
- [< Dolphin > emulator PC lightgun aiming (for Ghost Squad, etc)](#-dolphin--emulator-pc-lightgun-aiming-sample-config)
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

### Option 1: Lightgun emulation replacing mouse pointer

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

If you have installed a lightgun or arcade plugin (like [this](https://steamcommunity.com/app/1694600/discussions/0/3271312219438716734/) or [this](https://github.com/argonlefou/HotdRemake_ArcadePlugin/)), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and change the key assignments according to the plugin.

With either config, switch to motion pointer mode before starting the game, then in game options, set controller type to Keyboard/Mouse, sensitivity to 1.0, crosshair speed to 1.00 (some settings may be unavailable in arcade plugin).

<br>

## < Panzer Dragoon: Remake > PC gyro aiming sample config

Use the same config file as < The House of the Dead 2: Remake >, and change the key assignments to match the game. But the game has forced mouse smoothing, you need to move the controller slowly.

<br>

## < The Typing of the Dead: Overkill > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys to suit the game.

<br>

## < The House of the Dead III > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys to suit the game.

<br>

## < The House of the Dead 2 > PC lightgun aiming sample config

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys to suit the game. In game's config, select Mouse + Keyboard for player controller.

<br>

## < House of the Dead: Scarlet Dawn > PC lightgun aiming sample config

For TeknoParrot, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Back: Gamepad Back/View
<br>
Touchpad - West: Gamepad LB, North: Gamepad B, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to XInput, uncheck General - Windowed, check General - HideCursor, check Crosshairs - Enable Native. In controller setup, set the mapping by pressing the buttons on Gear VR controller. For easier input during setup, set motion pointer speed to 1 and dead zone to 10000 in app, then for Player 1, set Start by pressing Back, Gun Trigger by Trigger, Sub Trigger by Touchpad North, Controller Select by Touchpad West. Set dead zone back to 15 (default) and press Touchpad South to reset stick, then set Player 1 Gun X by pointing the controller rightward slowly until X+ is shown, set Gun Y by pointing upward until Y+ is shown.

Adjust the motion pointer speed to around 8~12 for the game.

<br>

## < MAME > emulator PC lightgun aiming sample config

For games like Time Crisis and Virtua Cop, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 5, Touchpad Center: Mouse right button, Touchpad South: Pointer reset

If you want to use non-press Touchpad for pedal, modify KeyTouchDirectCenter in the config file from Unassigned to Mouse right button (and restart app, text editor needs to be run as admin).

In MAME game's input device options, set lightgun and pedal device assignments to lightgun, keyboard input provider to dinput, lightgun input provider to win32.

<br>

## < Cxbx-Reloaded > emulator PC lightgun aiming sample config

For games like Virtua Cop 3, follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Home: Gamepad Start/Menu
<br>
Touchpad - Center: Gamepad B, West: Gamepad X, North: Gamepad LT, South: Pointer reset

In Cxbx-Reloaded input settings, select MS Gamepad S, click Configure, set Device to XInput/0/Gamepad, load Default Bindings, then give the Profile a name and Save.

<br>

## < TeknoParrot > emulator PC lightgun aiming sample config

### Option 1: Lightgun emulation replacing mouse pointer (e.g. Operation GHOST)

Follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys for example:

Trigger: Mouse left button, Back: 1, Home: 5
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, North: Mouse X1 button, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to RawInput, check General - Windowed, check General - HideCursor. In controller setup, set the mapping by pressing the buttons on Gear VR controller, set Coin 1 by pressing Home, for Player 1, set Start by pressing Back, Action by Touchpad North, Change by Touchpad West, Gun Trigger by Trigger, Reload by Touchpad Center, set Light Gun to Unknown Device.

Patch the game to correct screen resolution by [OpGhost_ResChanger](https://forum.arcadecontrols.com/index.php/topic,149714.msg1673148.html#msg1673148).

For games like The House of the Dead 4 without in-game crosshair, copy crosshair images P1.png and P2.png to folder of the game startup program, and check Crosshairs - Enable and Crosshairs - Scaling in game settings. But if the player 2 crosshair is shown even when not playing, rename P2.png to something else to hide it.

### Option 2: Lightgun emulation replacing gamepad left stick (e.g. Time Crisis 5)

Follow the instructions of [lightgun emulation option 2](#option-2-lightgun-emulation-replacing-gamepad-stick), and assign keys for example:

Trigger: Gamepad A, Home: Gamepad Start/Menu
<br>
Touchpad - North: Gamepad B, West: Gamepad LB, East: Gamepad RB, South: Pointer reset

In TeknoParrotUI game settings, set General - Input API to XInput, check Crosshair - Enable, uncheck General - Windowed. In controller setup, set the mapping by pressing the buttons on Gear VR controller. For easier input during setup, set motion pointer speed to 1 and dead zone to 10000 in app, then set Coin by pressing Home, Gun Trigger by Trigger, Gun Button by Touchpad North, Left Pedal by Touchpad West, Right Pedal by Touchpad East. Set dead zone back to 15 (default) and press Touchpad South to reset stick, then set Player 1 Gun X by pointing the controller rightward slowly until X+ is shown, set Gun Y by pointing upward until Y+ is shown.

Adjust the motion pointer speed to around 8~12 for the game.

For games like Silent Hill: The Arcade without in-game crosshair, copy crosshair images P1.png and P2.png to folder of the game startup program, and check Crosshairs - Enable and Crosshairs - Scaling in game settings.

<br>

## < RPCS3 > emulator PC lightgun aiming sample config

For PS3 games like Time Crisis: Razing Storm (Time Crisis 4 Arcade Ver, Razing Storm, Deadstorm Pirates), follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In RPCS3 game's GPU configuration, set Framelimit to Auto, check Write Color Buffers (required to fix screen brightness), check VSync. In I/O tab, set Mouse Handler to Basic, Move Handler to Mouse, Camera Input to PS Eye, Camera Handler to Fake, check Show PS Move Cursor. In Advanced tab, set VBlank Frequency to 59 Hz, uncheck VBlank NTSC Fixup (only available in game custom configuration, and it's important in order to get correct mouse button response).

In Mice->Basic Mouse configuration, set Button 1/2/3/4/5 to Mouse Left/Right/Middle/Back/Fwd respectively, set Button 6/7/8 to 6/7/8 (without Num+) respectively. In USB Devices->PS Move (Mouse) configuration, set Start/Select/Triangle/Circle/Cross/Square/Move/T to Mouse 7/6/4/5/2/3/8/1 respectively, and clear all other buttons. In Gamepad configuration, setup a keyboard or gamepad handler for PS3 Controller in order to navigate menus in game, as RPCS3 doesn't support PS Move navigation. When using a keyboard handler, use Ctrl-F11 in game to switch between PS3 Controller mode and PS Move mode.

In the crosshair calibration screen, make sure PS Move mode is active. Keep in window mode and resize the window as large as possible at the center of the screen while matching the game's aspect ratio (required to align the Windows cursor with the PS Move cursor).

For Time Crisis 4 and Razing Storm, press Trigger to start calibration. Except the center target, you should shoot each target at a little further from the outermost ring toward the window edge to get the correct calibration. But don't shoot too far, otherwise you can't turn left/right in the game when you need to point the crosshair to the window edge. For Deadstorm Pirates, press Back button to start calibration, just shoot at the center of each target.

Press Touchpad East to retry, or press Touchpad North to confirm, then Touchpad East to go back to title screen. Press Touchpad Center to select menu items and start a new game. Make sure the player controller is set to Motion Controller No.7.

After calibration, you can uncheck Show PS Move Cursor in I/O configuration. Optionally hide the Windows cursor by [nomousy](https://www.autohotkey.com/board/topic/2083-nomousy-disablehide-your-mouse-pointer-cmd/) ([download](https://www.mediafire.com/file/oglzpabl50b8juq/nomousy.zip/file)), run "nomousy /hide" to switch the Windows cursor on/off.

<br>

## < PCSX2 > emulator PC lightgun aiming sample config

For PS2 games like Time Crisis 3, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys for example:

Trigger: Mouse left button, Back: 8, Home: 7
<br>
Touchpad - Center: Mouse right button, West: Mouse middle button, East: Mouse X2 button, North: Mouse X1 button, South: Pointer reset

In PCSX2's Emulation settings, check Vertical Sync. In Graphics settings, check Show Overscan (required for some old games). In Controller settings -> USB Port 1, select GunCon 2. In Bindings tab, set Trigger to Pointer-0 Left Button, Shoot Offscreen to Pointer-0 Right Button, Calibration Shot to Keyboard 8 (without Numpad), set Buttons A/B/C/Start/Select to Pointer-0 Middle Button, Pointer-0 Button5, Pointer-0 Button4, Keyboard 7, Keyboard 6 respectively, set D-Pad Up/Down/Left/Right to Keyboard Numpad8/5/4/6. In Settings tab, set a crosshair png image in Cursor Path, check Manual Screen Configuration, set X Scale to 90%, Y Scale to 97% (different for some games, try around 92% to 97%), Center X to 400px, leave others to default.

For games like Resident Evil: Dead Aim which require the D-pad to work, you can map non-press Touchpad to D-pad keys by modifying KeyTouchDirectNorth/South/West/East from Unassigned to Numeric keypad 8/5/4/6 in the config file (and restarting app, text editor needs to be run as admin). Also change other assignments to suit the game.

If the custom crosshair image doesn't show up, it may be a bug of PCSX2. Try to modify Cursor Scale in the GunCon 2 Settings tab to fix. Press Alt-Enter to switch to fullscreen mode.

In the calibration screen, press Back button to start calibration. When finished, press Touchpad East to confirm (or follow game's intructions).

<br>

## < Dolphin > emulator PC lightgun aiming sample config

For Wii games like Ghost Squad, follow the instructions of [lightgun emulation option 1](#option-1-lightgun-emulation-replacing-mouse-pointer), and assign keys for example:

Trigger: Mouse right button, Back: Q, Home: E, +: 1, -: 2
<br>
Touchpad - Center: Mouse left button, West: Left arrow, East: Right arrow, North: Mouse middle button, South: Pointer reset

In Dolphin's Configuration -> Interface, set Mouse Cursor Visibility to Always. In Graphics settings, check V-Sync. In Controller settings, under Wii Remotes section, select Emulate the Wii's Bluetooth adapter, set Wii Remote 1 to Emulated Wii Remote. Click Configure, set Device to DInput/0/Keyboard Mouse, then click Default. In Motion Simulation tab, under Pointer section, set Vertical Offset to 15 cm, set Total Yaw to 19 degree (different for some games, try around 15 to 19 degree), set Total Pitch to 19 degree (different for some games, try around 11 to 19 degree), then Close the settings. Don't click Calibrate, it doesn't work.

For games like Resident Evil: The Umbrella Chronicles which use the Nunchuk stick, you can map non-press Touchpad to Nunchuk stick keys by modifying KeyTouchDirectNorth/South/West/East from Unassigned to W/S/A/D in the config file (and restarting app, text editor needs to be run as admin). Also change other assignments to suit the game.

Some games use shake to reload, it's mapped to mouse middle button (Touchpad North) by default.

After starting the game, if the crosshair moving scale is incorrect, try to adjust Total Yaw or Total Pitch in Controller settings. When ready, set Mouse Cursor Visibility to Never in Interface configuration. Press Alt-Enter to switch to fullscreen.

<br>

## Backup of user config

You can backup the user config file for different settings or game profiles. Exit the app first and it's inside a sub-sub folder in %LOCALAPPDATA%\Gear_VR_Controller

<br>

## Hints on low input lag for games and emulators

- Turn on game mode of TV or monitor if available
- Turn on low latency mode or anti-lag of GPU driver
- Keep the controller within good coverage of Bluetooth

