# VRPuppetHands

Active ragdoll type VR hands in Unreal Engine 5.4 using experimental Physics Control feature. Built on top of [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample)

This is not a production asset, more like an experimental proof of concept/set of examples to see how Physics Control based hands would feel and play in VR. You're welcome to play with it and use it however you see fit, as long as you respect license terms

## Showcase

youtubelink

## Installation

- Download [VR Expansion Plugin Example Template](https://github.com/mordentral/VRExpPluginExample) for UE 5.4 and follow setup instructions
- Drop contents of this repo into your project folder
- Run

## Notes
- Some files from Example Template were modified, so expect several random things to be broken/different - please don't report issues with this project to original repo
- Async Physics Tick and Substepping Async settings are enabled, which is said to be bad because it introduces latency. But otherwise I couldn't figure out a tick timing configuration that wouldn't cause hand to lag behind gripped interactable. I also seemingly couldn't achieve a higher tick rate without async settings, and default was rather janky. If you do know how to fix these, I would be happy to check out a PR or an Issue describing your solution
- Disclaimer: no guarantees in terms of active development/maintenance/support

## Credits

- [VR Expansion Plugin](https://github.com/mordentral/VRExpansionPlugin) and [Example Template](https://github.com/mordentral/VRExpPluginExample) by MordenTral
