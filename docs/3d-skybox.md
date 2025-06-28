# 3D Skybox

## Camera Stacking Setup

- You need to have a second camera in your scene for rendering the 3D skybox - an overlay camera, that has its culling mask set to the layers which house the 3D skybox objects.
- That camera needs to be added to the Camera Stack of the Main Camera
- The Skybox Camera script needs to be added to the overlay camera to make it rotate together with the main camera
- The Skybox objects need to be moved to a distance that will not intersect with any scene objects (Could use something that matches the far clip plane)

## Known Issues

- Star Corona and Gas Giant Glow effects break when drawn very far away.