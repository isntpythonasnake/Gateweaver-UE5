# Gateweaver
**A portal creation kit plugin for Unreal Engine 5.5+**

Ever wanted to make a warp gate, a Valve's Portal-esque game, a mirror into another dimension, or even a simple CCTV... TV without going into code?

Gateweaver is a powerful yet simple UE5 plugin that brings seamless "portal" mechanics to any project. Create fully functional portal that allow players to see, move, and interact across different spaces in real time using Render Target. It works right out of the box without fiddling with any settings.

## Features
- Create seamless portal pairs or portals with multiple entry/exit points using simple in-editor configuration.
  - Adjust mesh and texture of portal.
  - Portal type (pair or multiple). (Future feature)
- Portal can be spawned with collisions, object interactions, equipped tools, or point-and-click turrets.
- Allow/disallow types of surfaces where portals may or may not spawn, such as terrain surfaces.
- Objects or collision boxes that deletes portals.
- Add a customisable loading screen for long distance portals.
- Physics are fully translated between portals. Throw an object into one portal and it comes flying out through the other!

## Getting Started
### Installation


### Setting Up
<details>
<summary>Portal Setup</summary>

Portals need to be in pairs in order to work, obviously! Drag 2 portals into the game world. In the details panel of each portal, select the Exit Portal as the other portal. This will automatically teleport the player to the other portal when they step into one.
</details>

