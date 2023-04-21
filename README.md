# Bike Binder VR
A tool to physically control Riders Republic from a bike trainer and VR setup. 

POV Gameplay video : https://www.youtube.com/watch?v=0u8q5vU9P38


## Things you'll need :
- Download the .zip of the app here : https://github.com/Holydh/BikeBinderVR/releases/tag/Release
- .Net 6 runtime : [https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.16-windows-x64-binaries](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.16-windows-x64-binaries)
- A PCVR setup (only tested on Quest 2 with Airlink so far)
- Riders Republic
- a VR viewer like the free Depth3d companion app to see your desktop inside your hmd (https://github.com/BlueSkyDefender/Depth3D)
- A bike (even a dirt cheap one, it just needs to be compatible with the trainer) with it's stem screw removed so you can freely move the handlebar without moving the wheel (grease the base of the handlebar so it won't damage the stem).
- A bike trainer (there's some really cheap on second hand market too, mine was 30 bucks and works wonderfully well. No need for a connected one).

The app will automatically prompt you with Vigem Bus installer if you don't have it installed already at first launch. (The driver used to create the virtual Xbox gamepad)

### Please open an issue on this github page if you find bugs so I can keep track and fix them asap.

### Browse the right panel tabs of Bike Binder VR to find every info needed. Tutorial available in the "How to use" tab.

![1](https://user-images.githubusercontent.com/109091343/233663790-688885fc-62c7-4f99-aab9-b1e2da8abb82.png)


## A few more info :

- It's usable only for bike trainers where you can move the handle bar for now. I'll try to add a toggleable setting to control the bike by keeping the right controller in hand and using the joystick like a normal gamepad soon for people with standard indoor bike.

- You can use it for exercise but also just for fun by calibrating the pedaling intensity to your liking. So for people afraid of sweat in VR, you can calibrate it on the lowest speed possible and still have fun. It's also playable by having the hmd set aside, point it toward you so it can track at least the right controller on your handle bar, put a cloth inside it so it won't turn off and play on your normal TV/screen. But of course, this app is developped firstly for VR use.

- This software only takes care of the controls part. The VR view is handled by third party software of your choice but I suggest the free Depth3d companion app available here : https://github.com/BlueSkyDefender/Depth3D. It works perfectly with my app and is already real fun even without 3D.
For 3D view, you'll have to use VorpX or Reshade. More on that below.

- Since I only have a Quest 2 here, I tested the steamVR part with it. It should work well on other hmd but if not, feel free to open an issue about it on Github.

- There may be some physical limits with some controllers. Meaning, the Q2 controller fits nicely on the handle bar but I'm not so sure that every controllers will fit as nicely as these one (index controllers look a bit huge). Feel free to experiment and give me feedback, if I can change and adapt some stuff for specific hmds I'll try my best.


## For 3D rendering :
VorpX and Reshade works well with Riders Republic BUT, you'll have to force disable Battleye anticheat for this to work.

#USE AT YOUR OWN RISKS
## I would advise against it since this could probably get you banned. I don't know how tolerant Battleye and Ubisoft are toward VorpX and Reshade's hooking methods.

But if you want to try it anyway, there's a way to play only in Zen mod offline. Here's a quick how to :
- Set Ubisoft Connect in offline mod.
- Disable auto Updates on Riders Republic in Ubisoft Connect (in case they patch it soon, wich could happen quickly)
- In the game's root folder, rename "RidersRepublic_BE.exe" into "RidersRepublic_BE.exe.old"
- Duplicate RidersRepublic.exe and rename that copy into "RidersRepublic_BE.exe"
- Rename the folder "BattlEye" into "BattleEye.old"
- Just to be safe, add Firewall rules to block both RidersRepublic_BE.exe and RidersRepublic.exe

To play online again, just redo this list in reverse.



## A few final words :
I know I'm not objective but, damn, it's really fun to use, I'm really glad with how it turned out. I hope you'll enjoy it too.

## Wanna support my weird experiments ?
You can toss me a coin for a beer here : https://ko-fi.com/holydh


## Credits :
Vigem for gamepad inputs

Ab3d Oculus C# Wrapper for Oculus SDK

OvrSharp C# Wrapper for OpenVR

Licences available for all these libraries in the Licences folder.

