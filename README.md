# Gateweaver
**A portal creation kit plugin for Unreal Engine 5.5+**

Ever wanted to make a warp gate, a Valve's Portal-esque game, a mirror into another dimension, or even a simple CCTV... TV without going into code?

Gateweaver is a powerful yet simple UE5 plugin that brings seamless "portal" mechanics to any project. Create fully functional portal that allow players to see, move, and interact across different spaces in real time using Render Target. It works right out of the box without fiddling with any settings.

## Features
- Create seamless portal pairs or portals with multiple entry/exit points using simple in-editor configuration.
  - Adjust mesh and texture of portal.
  - Portal type (pair or multiple).
- Portal can be spawned with collisions, object interactions, equipped tools, or point-and-click turrets.
- Allow/disallow types of surfaces where portals may or may not spawn, such as terrain surfaces.
- Objects or collision boxes that deletes portals.
- Add a customisable loading screen for long distance portals.
- Physics are fully translated between portals. Throw an object into one portal and it comes flying out through the other!

## Getting Started
### Installation


### Setting Up
<details>
<summary>Render Targets Setup</summary>
  
**Forewarning:** I'm unable to automatically create render targets using Blueprints, a limitation of Blueprints unfortunately. You will have to create it yourself through my step-by-step tutorial below. Don't worry, it's fairly easy.

You're going to need **1 Render Target and 1 Material** for the render target per portal. This tutorial was made for only one portal! **Do the same steps for your exit portal as well.**
1. Right click on your project folder in the content browser and create a new **Render Target 2D**. Name it something recognisable like *RT_Portal_Entry_A*. Leave it untouched.
<img width="535" height="391" alt="Screenshot 2025-10-08 205520" src="https://github.com/user-attachments/assets/400d493c-1a33-4158-baf7-b94599171f84" />

2. Right click on your project folder again and create a new **Material**. Name it based on your render target like *M_Portal_Entry_A*. Double click on the new material to open it.
   
3. In the details panel of the material, change the **Material Domain** to **User Interface**.
<img width="564" height="303" alt="Screenshot 2025-10-08 210308" src="https://github.com/user-attachments/assets/463f2898-d4a0-453d-a61b-9711738c6140" />

4. In the material graph of said material, right click and add a **Texture Sample**. Connect **RGB** to **Final Color**.
<img width="340" height="236" alt="image" src="https://github.com/user-attachments/assets/a036dff8-cae4-4a11-b7a1-3efa788eeabe" />
<img width="624" height="345" alt="image" src="https://github.com/user-attachments/assets/56318cd3-172d-4529-ac4b-3eabc8a9448d" />

5. Double click on the black square of the Texture Sample and in the details panel, change the Texture to the Render Target 2D you just created.
<img width="516" height="435" alt="image" src="https://github.com/user-attachments/assets/c2ad763a-7c88-488b-9d5c-4bdd830d7106" />
<br/><br/>
Congratulations! You now have a Render Target and a Material! Drag a portal actor into the game world and plug these 2 objects into the respective render target and portal material slots.

</details>

