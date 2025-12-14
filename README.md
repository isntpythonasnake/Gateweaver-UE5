# Gateweaver
**A portal mechanics suite plugin for Unreal Engine 5.5+** `Release v2.0`

# The plugin is released!
Create portals, physics cube spawner (for portal interactions or more), portal gun, portal trigger boxes for hiding/showing portals. May also include a camera system that transitions cameras for live cinematics. Portals are fully equipped with physics and momentum.

## Features
- Create seamless portal pairs using simple in-editor configuration.
- Portal gun to aim and spawn portals on allowed surfaces using a custom "PortalPassthrough" collision channel.
- Objects spawner to spawn a physics cube for button interactions.
- Portal can be spawned with the portal gun or any other collisions, object interactions, equipped tools, or point-and-click turrets. Simply using a neat event!
- Allow/disallow types of surfaces where portals may or may not spawn, such as uneven surfaces.
- Other actors that hides/unhides portals.
- Momentum. The function of mass and velocity is conserved between portals. In layman's terms, speedy thing goes in, speedy thing comes out!

## Limitations
- As Unreal Engine render pipeline isn't recursive by default, other portals' render target will appear as black. Manually simulating this is performance heavy and would only work if only two portals are spawned. However as it happens, I found a way to make it so that render targets will only actively render when the player has the portal in view, except this won't likely be in the plugin at this time as it's not in my list of priorities.

## Getting Started

### Everything's been moved to the Wiki! 
https://github.com/isntpythonasnake/Gateweaver-UE5/wiki
