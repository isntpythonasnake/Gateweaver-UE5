# Gateweaver
**A portal creation kit plugin for Unreal Engine 5.5+**

Ever wanted to make a warp gate, a Valve's Portal-esque game, a mirror into another dimension, or even a simple CCTV... TV without going into code?

Gateweaver is a simple UE5 plugin that brings seamless "portal" mechanics to any project. Create fully functional portals that allow players to see, move, and interact across different spaces in real time using Render Target. It works right out of the box without fiddling with any settings.

## Features
- Create seamless portal pairs or portals with multiple entry/exit points using simple in-editor configuration.
  - Adjust mesh and texture of portal. (Future feature)
  - Portal type (pair or multiple). (Future feature)
- Portal can be spawned with collisions, object interactions, equipped tools, or point-and-click turrets.
- Allow/disallow types of surfaces where portals may or may not spawn, such as terrain surfaces.
- Objects or collision boxes that deletes portals.
- Physics are fully translated between portals. Throw an object into one portal and it comes flying out through the other!

## Things to note
There are a few limitations with this portal that I'm unable to resolve at this time:
1. ~~Portals have 2 collision boxes, PlayerNearby that detects when the player is near a portal, and PlayerTeleport teleports the player. The problem is the latter collision box has to be placed **behind** the portal to give the impression of walking into a portal. This means that you can't place portals directly on walls where physics collisions are enabled.~~

## Bugs
- ~~Camera tilted on the roll axis when the linked portal is rotated.~~
- ~~Camera flickers when player rotates their camera behind a portal.~~

## TODO
- [X] Portals can teleport player and keep their velocity, including launching players when entered with momentum.
- [x] Dynamic Render Target and materials for each portal actor spawned with its configurable settings.
- [x] Portals equipped with a panel to *hide* the other side and behave as a moveable object for actor interaction.
- [x] Allow user to use their own custom meshes and effects.
- [x] Portals can be spawned by another actor.
- [x] Transition an additional camera to make teleportation seamless for third person characters. (Target view with blend)
- [ ] Types of surfaces to allow or disallow portals spawning.
- [x] Objects or collision boxes that deletes portals.
- [ ] Toggle disable render targets for portals that aren't in view (Lag).
- [ ] Other Actors teleport interactions with portal.

## Getting Started
### Installation


### Setting Up
<details>
<summary>Portal Setup</summary>

Portals need to be in pairs in order to work, obviously! Drag 2 portals into the game world. In the details panel of each portal, select the Exit Portal as the other portal. This will automatically teleport the player to the other portal when they step into one.

New portals will look like this. Don't be too intimidated by the black textures.
<img width="1320" height="909" alt="image" src="https://github.com/user-attachments/assets/d5b5bcd7-d467-4ddc-9f9a-b6396acfe3f2" />

In the details panel of said portal, you'll find the Portal Setup category with: Exit Portal, Panel Colour, and Frame Colour. 
1. The colours don't correspond to the exit portal, meaning you have the freedom to colour them however you wish! Point the Exit Portal to the destination portal.
2. Panel colour: Colour of the portal's panel.
3. Frame colour: Colour of the portal's noisy border.



</details>

