# Procedural Celestial Body Materials Samples

## Installation
The assets for the 3D gas giants and stars are stored in a separate folder, as they are currently being distributed as a free asset on the asset store. They are included in the paid Procedural Space Skybox Asset, and do not require a separate download.

## Samples
There are two sample scenes in this asset:

- Space Objects Sample Scene - shows 6 sample celestial bodies - 3 stars and 3 gas giants.
- 3D Skybox Sample Scene - shows a 3D Skybox set up using some of the celestial body prefabs.

## URP Settings

![URP Settings Project](../assets/images/3d-skybox/3d-skybox-renderer-asset.png)

The Sample URP Asset and Renderer have the shadows and anti-aliasing settings used to get the look of the asset presented in the store page.

The 3D Skybox Renderer is related to [3D Skybox](../3d-skybox.md) setup.

## VSync

To avoid screen tearing with the glowing corona post-processing effect, make sure to enable VSync in the Scene View:

![Scene VSync Settings](../assets/images/procedural-celestial-bodies/scene-vsync.png)

And in Builds, from the Project Settings:
![Build VSync Settings](../assets/images/procedural-celestial-bodies/build-vsync.png)

