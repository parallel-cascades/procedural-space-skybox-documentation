# 3D Skybox Background

## Introduction

A 3D Skybox allows you to have giant stellar bodies in the background of your scene, that get rendered behind everything and do not affect the gameplay or physics of the world, but provide a cosmic sense of scale.

There are different ways to implement this, but the approach chosen for this asset uses custom passes and stencil overrides, instead of multiple cameras. This approach is more performant and less bug prone.

Here's how the effect looks with opaque celestial bodies with transparent elements in the background:
![3D Skybox GIF](./assets/images/3d-skybox/3d-skybox.gif)

And here's a guide to how the objects are actually set-up:
![3D Skybox Layers Guide](./assets/images/3d-skybox/3d-skybox-objects.png)

## Setup

### Layers

To have your objects become part of the 3D Skybox in a scene, they need to be part of the 3D Skybox layer:
![3D Skybox Inspector Layer Selection](./assets/images/3d-skybox/3d-skybox-layers.png)

### URP Asset
The actual overriding of render order and stenciling is set up in a sample URP Renderer asset located in the `Samples` folder:
![3D Skybox URP Renderer Location](./assets/images/3d-skybox/3d-skybox-renderer-asset.png)

The settings of the skybox renderer should look like this:
![3D Skybox Renderer Inspector](./assets/images/3d-skybox/3d-skybox-renderer-inspector.png)

This renderer is automatically loaded when you open the 3D Skybox Sample Scene.

### Additional Directional Light

If you want your 3D Skyboxes to support shadows and to not receive or cast shadows on scene objects, they need to be excluded from the main directional light's culling mask, and a second directional light needs to be added just for the 3D Skybox layer. Then scene objects only cast and receive shadows from scene objects, and 3D skybox objects cast and receive shadows only from other 3D skybox objects.

![Directional Light Hierarchy](./assets/images/3d-skybox/light-setup.png)
/// caption
A simple setup is to parent the 3D skybox directional light to the main directional light.
///

![Culling Mask Setup](./assets/images/3d-skybox/light-culling-mask.png)
/// caption
Main light excludes the 3D Skybox layer; 3D Skybox light excludes everything BUT the 3D Skybox layer.
///






