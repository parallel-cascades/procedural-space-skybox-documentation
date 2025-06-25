# Shader Skybox Introduction

The procedural skybox shader is versatile but performance heavy skybox solution. It uses various procedural noise techniques to generate natural looking space components - fields of stars, nebula clouds, suns and a galactic band.

Its main benefit is its customisability - all of the skybox components are modular and adjustible, allowing infinite skybox variants. Have a look at some of the sample images below:

| ![Shader Skybox Example 1](../assets/images/shader-skybox-examples/shader_skybox_examples_001.png) |
|:--:|
| Example 1: A starfield with small star dots with varied colors and sizes. Fewer, larger, glowing stars can be seen. Dominating the view is a large luminous galactic band, with a far denser star field, and a soft blue glow spreading from its edges.|

| ![Shader Skybox Example 2](../assets/images/shader-skybox-examples/shader_skybox_examples_002.png) |
|:--:|
| Example 2: The colors of the galactic band are altered, the starfield now has a faded, red glow, and the blue glow is transformed into a sickly green cloud. |

| ![Shader Skybox Example 3](../assets/images/shader-skybox-examples/shader_skybox_examples_003.png) |
|:--:|
| Example 3: Back to the original blue galaxy, it can be rotated to lie on a 'horizontal' plane (of course, there is no horizon in space). |

| ![Shader Skybox Example 4](../assets/images/shader-skybox-examples/shader_skybox_examples_004.png) |
|:--:|
| Example 4: The galaxy effect size can be reduced, creating a smaller galactic disk, or one that is further away from the observer. |

| ![Shader Skybox Example 7](../assets/images/shader-skybox-examples/shader_skybox_examples_007.png) |
|:--:|
| Example 5: The galactic band effect can be completely disabled, revealing some faint reddish nebulas that were previously obscured. |

| ![Shader Skybox Example 8](../assets/images/shader-skybox-examples/shader_skybox_examples_008.png) |
|:--:|
| Example 8: Increasing the glow of the nebulas shows their natural patterns much more clearly. |

| ![Shader Skybox Example 9](../assets/images/shader-skybox-examples/shader_skybox_examples_009.png) |
|:--:|
| Example 9: Individual control of the random seed used for the nebula shape noise algorithm allows us to create new nebula shapes.  |
