# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.0.1] - 2025-06-27

- Added
    - Links to new online documentation.
    - New sample scene showcasing how to combine both skybox effects.

- Changed
    - Disabled depth write on both procedural skybox shaders, to prevent depth conflicts with the VFX Graph skybox effect.

- Fixed
    - Reconnected disconnected nodes in the VFX Graph skybox effect for nebula rendering.
    - The Procedural Sun module in Procedural Space Skybox and Cubemap Skybox with Procedural Sun would get misaligned when moving the camera. 
    - Sun Distance (internal property) value was set too low, causing the shimmer effect to become misaligned with the sun core in the skybox when moving the camera. A larger default value has been set to prevent this issue.

## [3.0.0] - 2025-06-23

- Added
    - New, more performant procedural skybox technique using VFX Graph.
    - Editor tools for creating star and nebula textures, and baking them into texture arrays.
    - New welcome window with links to sample scenes and documentation.

- Changed
    - Asset format reverted to Assets folder package. This will require uninstalling any previous versions of the package.


## [2.0.0] - 2024-10-21

- Changed
    - Updated to work with Unity 6000.0
    - Asset format updated to Unity Package Manager (UPM) format. This will require uninstalling any previous versions of the package.
    - Inspector shader group name changed from "Shader Graphs/" to "Parallel Cascades/"
    - Cubemap Rendering automatically applies import settings to generated cubemap assets.

- Removed
    - Legacy cubemap rendering - individual textures for 6-sided cubemap shader and legacy cubemap asset.

## [1.1.0] - 2024-10-12

- Added
    - Added Procedural Sun effect to Procedural Space Skybox shader.
    - Added Cubemap Skybox with Procedural Sun shader.
    - Added boolean keywords for each effect - nebula, sun, stars, galaxy.
    - Added dropdown to select whether to save skybox as a cubemap asset or as a 6 individual textures.
    - Assembly definitions for common runtime and editor code.

- Changed
    - Updated documentation to include new features.
    - 'Render Cubemap to Skybox' menu has been moved from 'Component/' to 'Tools/' toolbar menu.
    - Cleaned up some code comments.
    - Editor focuses on saved asset after rendering skybox.

- Removed
    - Removed 'package.json' file from asset root.

## [1.0.0] - 2024-09-09

- Initial release