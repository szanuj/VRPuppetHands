# VRPuppetHands

Active ragdoll (puppet) type VR hands in Unreal Engine 5.4 using experimental Physics Control feature. Built on top of [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample)

This is a demo project I put together to see how active ragdoll (puppet) hands would feel in VR. 
Unreal Engine 5's Physics Control component makes puppets fairly simple to create, though there is a lot of fine tuning to do for a convincing effect. Scene contains a bunch of example physics-based interactables including a pettable cat - it is also a puppet, alas, not carryable.
Feel free to check out [dev build](https://github.com/szanuj/VRPuppetHands/releases/latest) or inspect project in Unreal (instructions below).

## YouTube Showcase

[![YouTube](http://i.ytimg.com/vi/QAPIu8JDILE/hqdefault.jpg)](https://www.youtube.com/watch?v=QAPIu8JDILE)

## Installation

- Download [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample) for UE 5.4 and follow setup instructions
- Close Unreal, drop contents of this repo into your project folder, choose "Replace all"

## Notes
- Some files from Example Template were modified, so things may be broken/different - please do not report issues with this project to Example Template repo
- Async Physics Tick and Substepping Async settings are enabled, introducing latency. But when I tried disabling these, it caused hand to visually lag behind gripped interactable. It's likely a tick timing configuration problem but I couldn't find a setup that worked. I also didn't manage to achieve a higher tick rate without async settings, and default was rather janky. If you do know how to fix these, feel free to propose a solution.
- This is just a what-if demo. Don't expect additional maintenance or updates

## Credits

- [VR Expansion Plugin](https://github.com/mordentral/VRExpansionPlugin) and [Example Template](https://github.com/mordentral/VRExpPluginExample) by MordenTral
