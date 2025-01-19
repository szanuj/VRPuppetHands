# VRPuppetHands

Active ragdoll (puppet) type VR hands in Unreal Engine 5.4 using experimental Physics Control feature. Built on top of [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample)

This is a demo project I put together to see how active ragdoll (puppet) hands would feel in VR. 
Unreal Engine 5's Physics Control component makes puppets fairly simple to create, though there is a lot of fine tuning to do for a convincing effect. Scene contains a bunch of example physics-based interactables including a pettable cat - it is also a puppet, alas, not carryable.

[Grab the dev build (Windows)](https://github.com/szanuj/VRPuppetHands/releases/latest) or inspect project in Unreal (instructions below).

Supports hand tracking on Quest 2 (you have to enable Developer Runtime Features in Meta Quest Link app) and finger curls on Valve Index controllers. There is no gesture detection (editor started crashing on startup whenever I added it) so for grabbing and teleport/snap turn you're gonna need to use controllers.

Also works without VR, in FPS mode (thanks to VREP Example Template). LMB for grabbing, 1-4 keys for different right hand finger curls.

## YouTube Showcase

[![YouTube](http://i.ytimg.com/vi/QAPIu8JDILE/hqdefault.jpg)](https://www.youtube.com/watch?v=QAPIu8JDILE)

## Project setup

- Download [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample) for UE 5.4 and follow setup instructions
- Close Unreal, drop contents of this repo into your project folder, choose "Replace all"

## Notes
- Some files from Example Template were modified, so things may be broken/different - please do not report issues with this project to Example Template repo
- Async Physics Tick and Substepping Async settings are enabled, introducing latency. But when I tried disabling these, it caused hand to visually lag behind gripped interactable. It's likely a tick timing configuration problem but I couldn't find a setup that worked. I also didn't manage to achieve a higher tick rate without async settings, and default was rather janky. If you do know how to fix these, feel free to propose a solution.
- This is just a what-if demo. Don't expect additional maintenance or updates

## Credits

- [VR Expansion Plugin](https://github.com/mordentral/VRExpansionPlugin) and [Example Template](https://github.com/mordentral/VRExpPluginExample) by MordenTral
