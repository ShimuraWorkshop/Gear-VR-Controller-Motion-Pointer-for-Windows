# Gear VR Controller Motion Pointer for Windows

![Screenshot](./screenshot.png "Screenshot")

Convert the Gear VR Controller into a PC air mouse, motion pointer, wireless presenter and gyro/motion gamepad.

Features
- No VR headset or mobile phone needed
- Wireless presenter, air mouse and motion pointer
- Key or action mapping to buttons and motions
- Combo editor for keys input
- Trackpad mouse cursor or scrolling
- Compass mode
- Quick and easy calibration of sensors

System requirements
- Windows 10 x64 or Windows 11
- .NET Desktop Runtime 9.0

Setup Guide
- No pairing needed, just turn on PC Bluetooth and install batteries to the controller
- Press any button on the controller, then click the Search icon in app
- Click the Connect button, that's it

Calibration for Motion Sensing and Motion Pointer
- Place the controller upside down on a stable surface, then click the CAL button, that's it

Download latest version

v2.1.11
[Link 1](https://drive.google.com/drive/folders/1FN2FOPHm6QyQqntdEFUnvLKOWFaLj8HI)
[Link 2](https://www.mediafire.com/file/mr4r299a5cj822j/Gear_VR_Controller_setup.exe/file)

SHA-256: 76eb62c4fd7f4da84400697364c6729f34198e0832e366cca77e7f8d696c6293

<br>

Gear VR is a trademark of Samsung Electronics Co., Ltd.

​Windows is a trademark of Microsoft Corporation

<br>

## *Secret* gyro/motion gamepad emulation in new version

Now you can use the controller like a gyro gamepad. Gyro aiming together with analog touch stick (needn't press) are supported. Gamepad buttons and sticks are added to key assignment list for mapping to touchpad press (8 directions, center and lower edge), other 5 buttons and 12 motions. For easier control, assign pointer toggle to a button.

To use the gamepad mode, install [ViGEmBus](https://github.com/nefarius/ViGEmBus/releases/tag/v1.22.0), edit the file "C:\Program Files\Gear VR Controller\Gear_VR_Controller.dll.config" (default) and restart the app.

Modify to False in the line under:

DefaultStabilizePointerClick

Modify to True in the lines under:

DefaultGameMode

DefaultGameKeyboardMode

DefaultGamePointerMode

DefaultEmulateGamepad

You can also map controller roll, pitch, yaw motions to stick axes or triggers to make it a motion gamepad. Try to adjust motion pointer speed to 1~3 and assign a pointer reset button. Explore more settings if you're interested.

Modify to True in the lines under:

DefaultGamepadUsePitch

DefaultGamepadUseYaw

Some games may work better with keyboard+mouse emulation, or if you want to combine its input with another gamepad, in that case, leave the DefaultEmulateGamepad option to False.

If the game is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

<br>

## < The House of the Dead 2: Remake > PC gyro aiming sample config

Config file
[Link](https://www.mediafire.com/file/ca3mrdhr4q8jl0g/Gear_VR_Controller.dll.config_the.house.of.the.dead.2.remake.zip/file)

ViGEmBus not required, update the app to v2.1.11, extract the config to "C:\Program Files\Gear VR Controller\" (default), then assign keys for example:

Trigger: Mouse left button, Back: Enter, Home: Tab, +: F, -: Esc

Touchpad - Center: Mouse right button, West: Q, East: E, South: Pointer temporary off, North: Unassigned

Touchpad (without press) is mapped to WASD by default, you can change it by modifying KeyTouchDirectNorth/East/South/West/Center in the config file (and restarting app) when necessary.

Switch to motion pointer mode before starting the game, then in game options, set controller to Keyboard/Mouse, aiming stick to Both Sticks, mouse sensitivity to 1.0, crosshair speed to 1.0.

If the game is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

This config file is also suitable for < Panzer Dragoon: Remake >, just change the key assignments to match the game. But the game has forced mouse smoothing, you need to move the controller slowly.

<br>

## < The House of the Dead: Remake > PC gyro/lightgun aiming sample config

Config file
[Link](https://www.mediafire.com/file/yxi0v4sfd9ypkyy/Gear_VR_Controller.dll.config_the.house.of.the.dead.remake.zip/file)

ViGEmBus not required, update the app to v2.1.11, extract the config to "C:\Program Files\Gear VR Controller\" (default), then assign keys for example:

Trigger: Mouse left button, Back: Enter, -: Esc

Touchpad - Center: Mouse right button, West: Q, East: E, North: F, South: Pointer temporary off

If you have installed a lightgun or arcade plugin (like [this](https://steamcommunity.com/app/1694600/discussions/0/3271312219438716734/) or [this](https://github.com/argonlefou/HotdRemake_ArcadePlugin/)), you can emulate lightgun aiming by modifying GamePointerUseRelativeMovement to False in the config file (and restarting app), then assigning Pointer reset to Touchpad South, also other keys according to the plugin, and adjusting the motion pointer speed in app.

Switch to motion pointer mode before starting the game, then in game options, set controller type to Keyboard/Mouse, sensitivity to 1.0, crosshair speed to 1.00.

If the game is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

The lightgun aiming config is also suitable for < The Typing of The Dead: Overkill >, just change the key assignments to match the game.

<br>

## < Panzer Dragoon: Remake > PC gyro aiming sample config

Use the same config file as < The House of the Dead 2: Remake >, and change the key assignments to match the game. But the game has forced mouse smoothing, you need to move the controller slowly.

<br>

## < The Typing of the Dead: Overkill > PC lightgun aiming sample config

Use the same config file as < The House of the Dead: Remake >, follow the instructions of lightgun aiming config, and change the key assignments to match the game.

<br>

## < MAME > emulator PC gyro aiming sample config

Use the same config file as < The House of the Dead: Remake > and modify ScaleRelativeMovement to 1000 (for 1:1 movement), in MAME game's input device options, change lightgun and pedal device assignments to mouse, change mouse input provider to dinput, then change the key assignments in app to match MAME emulator (need to keep "Pointer temporary off" assigned to a button).
