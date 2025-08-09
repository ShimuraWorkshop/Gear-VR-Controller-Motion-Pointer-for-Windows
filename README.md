# Gear VR Controller Motion Pointer for Windows

![alt text](https://github.com/ShimuraWorkshop/Gear-VR-Controller-Motion-Pointer-for-Windows/blob/main/screenshot.png "screenshot")


Convert the Gear VR Controller into a PC air mouse, motion pointer, wireless preseneter and gyro gamepad.


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
- Place the controller upside down on a steady surface, then click the CAL button, that's it


Download latest version

[Link 1](https://drive.google.com/drive/folders/1FN2FOPHm6QyQqntdEFUnvLKOWFaLj8HI)

[Link 2](https://www.mediafire.com/file/mr4r299a5cj822j/Gear_VR_Controller_setup.exe/file)


## *Secret* gamepad emu in new version

Now you can use the controller like a gyro gamepad. Gyro aiming together with analog touch stick (needn't press) are supported. Gamepad buttons and sticks are added to key assignment list for mapping to touchpad press (8 directions, center and lower edge), other 5 buttons and 12 motions. For easier control, assign pointer toggle to a button.

To use the gamepad mode, install ViGEmBus https://github.com/nefarius/ViGEmBus/releases/tag/v1.22.0, edit the file "C:\Program Files\Gear VR Controller\Gear_VR_Controller.dll.config" (default) and restart the app.

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

Some games may work better with keyboard+mouse emulation, in that case, leave the DefaultEmulateGamepad option to False.

If the game is run as admin, this app also needs to be run as admin, otherwise Windows won't let them work together.

## The House of the Dead 2 Remake sample config

Download

[Link](https://www.mediafire.com/file/ca3mrdhr4q8jl0g/Gear_VR_Controller.dll.config_the.house.of.the.dead.2.remake.zip/file)

Update the app to v2.1.10, extract the config to "C:\Program Files\Gear VR Controller\" (default), then assign keys for example:

Trigger: Mouse left button, Back: Enter, Home: Tab, +: F, -: Esc

Touchpad - Center: Mouse right button, West: Q, East: E, South: Pointer temporary off, North: Unassigned

Switch to motion pointer mode before starting the game, then in game options, set control to Keyboard+Mouse, set mouse sensitivity to 1.0. For better aiming, disable "Enhance pointer precision" in Windows mouse settings -> Additional mouse options -> Pointer Options

