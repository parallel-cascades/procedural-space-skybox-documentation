# Properties Reference

## Random Seed

All of the effects of this skybox shader are generated from pseudorandom noise functions. These are seeded with an initial value, out of which each unique variation is generated. There are several properties for random seeds for different effects:

| ![3D Random Seed Example](../assets/images/shader-properties-tutorial/3d-random-seed.gif) |
|:--:|
| The 3D Random seed affects background stars, nebulas and the galaxy band. Notice how the glowing stars remain stationary, as they use a different seed. Also notice how 'scrolling' the 3D seed in any direction makes the effects 'flow'. These noise algorithms are continuous functions, and small changes to the 3D seed shift the pattern in the designated direction. |

The galactic band and nebulas also have their own 3D seed variables, if you only want to alter those effects.

| ![Nebula Offset Example](../assets/images/shader-properties-tutorial/nebula-offset-seed.gif) |
|:--:|
| For nebulas, the property is named Nebula Offset, and there are 6 such properties, one for each side of the skybox cube. In the example Back Nebula Offset[-Z] is the nebula generated towards the -Z direction in 3D space. |

Glowing stars have their own integer seed, as they are generated in a different manner:

| ![Glowing Stars Seed](../assets/images/shader-properties-tutorial/glowing-stars-seed.gif) |
|:--:|
| Notice how the function here is not continous, so every new seed generates a totaly different star placement. |
