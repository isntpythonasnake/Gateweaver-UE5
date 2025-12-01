# Gateweaver
**A portal mechanics suite plugin for Unreal Engine 5.5+** `Beta v1.0`

# The plugin is 95% done! If you're from TD module, please feel free to test it because it's my first time packaging a plugin... it might break.

Ever wanted to make a warp gate, a Valve's Portal-esque game, a mirror into another dimension, or even a simple CCTV... TV without going into code?

Create portals, physics cube spawner (for portal interactions or more), portal gun, portal trigger boxes for hiding/showing portals. May also include a camera system that transitions cameras for live cinematics. Portals are fully equipped with physics and momentum.

## Features
- Create seamless portal pairs using simple in-editor configuration.
- Portal gun to aim and spawn portals on allowed surfaces using a custom "PortalPassthrough" collision channel.
- Objects spawner to spawn a physics cube for button interactions.
- Cinematic camera system triggered using events.
- Portal can be spawned with the portal gun or any other collisions, object interactions, equipped tools, or point-and-click turrets. Simply using a neat event!
- Allow/disallow types of surfaces where portals may or may not spawn, such as uneven surfaces.
- Other actors that hides/unhides portals.
- Momentum. The function of mass and velocity is conserved between portals. In layman's terms, speedy thing goes in, speedy thing comes out!

## Limitations
- As Unreal Engine render pipeline isn't recursive by default, other portals' render target will appear as black. Manually simulating this is performance heavy and would only work if only two portals are spawned. However as it happens, I found a way to make it so that render targets will only actively render when the player has the portal in view, except this won't likely be in the plugin at this time as it's not in my list of priorities.

## TODO
| Thing | Description | Completed? | Remarks |
| :------------: | :------------- | :------------: | :------------: |
| Portal | Portals can teleport player and keep their velocity, including launching players when entered with momentum. | ✔️ |
| Portal | Dynamic Render Target and materials for each portal actor spawned with its configurable settings. | ✔️ |
| Portal | Portals equipped with a panel to *hide* the other side or behave as a moveable object for actor interaction. | ✔️ |
| Portal gun | Portal gun that spawns portals in a set interval. | ✔️ |
| Portal gun | Types of surfaces to allow or disallow portals spawning. | ✔️ |
| Hiding portals | Actors that hide/unhide portals for lag reduction. | ✔️ | Lag reduction |
| Portal | Toggle disable render targets for portals that aren't in view. | ✔️ | Lag reduction |
| Physics actors | Other Actors teleport interactions with portal. | ✔️ | 
| Portal gun | Portal gun aim animation. |  | 

## Getting Started
### Everything's been moved to the Wiki! 
https://github.com/isntpythonasnake/Gateweaver-UE5/wiki
