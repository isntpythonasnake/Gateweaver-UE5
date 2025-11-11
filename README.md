# Gateweaver
**A portal creation kit plugin for Unreal Engine 5.5+** `Unreleased v0.12.11112025`

# The plugin is 90% done and should be released soon!

Ever wanted to make a warp gate, a Valve's Portal-esque game, a mirror into another dimension, or even a simple CCTV... TV without going into code?

Create portals, physics cube spawner (for portal interactions or more), portal gun, portal trigger boxes for hiding/showing portals. May also include a camera system that transitions cameras for live cinematics. Portals are fully equipped with physics and momentum.

## Features
- Create seamless portal pairs using simple in-editor configuration.
  - Adjust mesh and texture of portal. (Future feature)
  - Portal type (pair or multiple). (Future feature)
- Portal can be spawned with the portal gun or any other collisions, object interactions, equipped tools, or point-and-click turrets. Simply using a neat event!
- Allow/disallow types of surfaces where portals may or may not spawn, such as uneven surfaces.
- Other actors that hides/unhides portals.
- Physics are fully translated between portals. Throw an object into one portal and it comes flying out through the other!

## TODO
- [X] Portals can teleport player and keep their velocity, including launching players when entered with momentum.
- [x] Dynamic Render Target and materials for each portal actor spawned with its configurable settings.
- [x] Portals equipped with a panel to *hide* the other side and behave as a moveable object for actor interaction.
- [x] ~~Allow user to use their own custom meshes and effects.~~ (Bugged, future feature perhaps)
- [x] Portal gun that spawns portals in a set interval.
- [x] Transition an additional camera to make teleportation seamless for third person characters. (Target view with blend)
- [x] Types of surfaces to allow or disallow portals spawning.
- [x] Actors that hide/unhide portals for lag reduction.
- [x] Toggle disable render targets for portals that aren't in view for lag reduction.
- [X] Other Actors teleport interactions with portal.
- [ ] Portal gun aim animation

## Getting Started
### Installation


### Setting Up
<details>
<summary>Portal Setup</summary>

Portals need to be in pairs in order to work, obviously! Drag 2 portals into the game world. In the details panel of each portal, select the Exit Portal as the other portal. This will automatically teleport the player to the other portal when they step into one.

New portals will look like this. Don't be too intimidated by the unassuming textures.
<img width="1320" height="909" alt="image" src="https://github.com/user-attachments/assets/d5b5bcd7-d467-4ddc-9f9a-b6396acfe3f2" />

In the details panel of said portal, you'll find the Portal Setup and the Is Portal For Gun categories:
1. Point the Exit Portal to the destination portal.
2. Panel colour: Colour of the portal's panel. 
3. Frame colour: Colour of the portal's noisy border. The colours don't correspond to the exit portal, meaning you have the freedom to colour them however you wish!
4. Is Panel Hidden: By default, panels should be hidden unless you'd like to have them rotatable via an external actor like a button.
6. Is Portal For Gun?: Set to true if you'd like to link this portal to a portal gun.
7. BP Portal Gun: If (5) is set to true, select the portal gun to link this portal to.

WIP more details coming soon because im too preoccupied with the plugin i don't really have time for documentation writing lol

</details>

