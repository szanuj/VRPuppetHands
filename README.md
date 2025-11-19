# VRPuppetHands

Active ragdoll (puppet) type VR hands in Unreal Engine 5.4 using experimental Physics Control feature. Built on top of [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample)

This is a demo project I put together to see how active ragdoll (puppet) hands would feel in VR. 
Unreal Engine 5's Physics Control component makes puppets fairly simple to create, though there is a lot of fine tuning to do for a convincing effect. Scene contains a bunch of example physics-based interactables including a pettable cat - it is also a puppet, alas, not carryable.

[Grab the build (Windows)](https://github.com/szanuj/VRPuppetHands/releases/latest) or inspect project in Unreal (instructions below).

Supports hand tracking through OpenXR\*. Hand tracking mode will activate automatically when you put away controllers. There is no gesture detection (editor started crashing on startup whenever I added it) so grip and teleport/snap work only on controllers.

\* Hand tracking through Meta Quest Link no longer works after recent updates from Meta. In late 2024 it worked after you enabled Developer Runtime Features in desktop app. You can try your luck with Steam Link, Virtual Desktop or ALVR, but I haven't tested that. Finger curls on Valve Index controllers should just work.

Also works without VR, in FPS mode (thanks to VREP Example Template). LMB for grabbing, 1-4 keys for different right hand finger curls.

## YouTube Showcase

[![YouTube](http://i.ytimg.com/vi/QAPIu8JDILE/hqdefault.jpg)](https://www.youtube.com/watch?v=QAPIu8JDILE)

## Project setup

- Make sure you're using UE 5.4
- Download [VR Expansion Plugin Example Template (branch 5.4)](https://github.com/mordentral/VRExpPluginExample/tree/5.4-Locked) and follow setup instructions
- Close Unreal, drop contents of this repo into your project folder, choose "Replace all"

## Notes
- Some files from Example Template were modified, so things may be broken/different - please do not report issues with this project to Example Template repo
- Async Physics Tick and Substepping Async settings are enabled, introducing latency. But when I tried disabling these, it caused hand to visually lag behind gripped interactable. It's likely a tick timing configuration problem but I couldn't find a setup that worked. I also didn't manage to achieve a higher tick rate without async settings, and default was rather janky. If you do know how to fix these, feel free to propose a solution.
- This is just a what-if demo. Don't expect additional maintenance or updates

## Credits

- [VR Expansion Plugin](https://github.com/mordentral/VRExpansionPlugin) and [Example Template](https://github.com/mordentral/VRExpPluginExample) by MordenTral
