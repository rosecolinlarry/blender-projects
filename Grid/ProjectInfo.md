# Grid Floor

## Description

Uses curves to render the Blender default grid. Thickness of the lines is defined in `Scene > ViewLayer > Custom Properties > grid_bevel_depth`.

![image](images/Set%20Grid%20Bevel%20Depth.jpg)

## Purpose

While `View > Viewport Render Image` can render the grid floor and axes in Eevee, when using Cycles, the objects do not render properly. It loses the sphere object and HDRI.

This uses curves to fake the viewport's grid to enable rendering of it. The grid lines' Ray Visibility is set to "Camera" and nothing else. This means it casts no shadow, reflection, will not affect other objects, etc.

Viewport in Render View:
![image](images/Viewport%20Screen%20Shot.jpg)

Using Viewport Render Image:
![image](images/Viewport%20Render%20Image.png)

Using Render with the Grid Collection:
![image](images/Render%20Image.png)

## Materials
- "Dispersion Glass" by "DJ SOLANA" and can be imported using blenderkit. Direct link [here](https://www.blenderkit.com/get-blenderkit/af93763d-1343-48ac-b181-1c2846a4372b/).
- "Shadeless - *": Blender no longer has the "Shadeless" option for materials. This replicates the effect.

## Default View

Included the default cube, it is just hidden. The camera is in the blender default location.

Render of just the grid curves:
![image](images/Default%20Scene%20-%20Only%20Grid.png)

