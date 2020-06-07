# Final Project Proposal
Peihua Huang and Jackie Lin (pd 10)

## Features
We will be implementing the following features in our project:
- light
    ```
    light lightname r g b x y z #creates a light with rgb values r, g, b at location x, y, z
    light lightname r g b x y z [knob] [x_axis] [y_axis] [z_axis] #creates a moving light that starts moving from location x, y, z
    #if any of the axis is set to 0, the light will not move on that axis, if it's set to 1, the light will move
    ```
  - existing MDL command
  - will add light to symbol table
  - all lights will be used in calculating diffuse and specular reflection
- mesh
  - existing MDL command
  - will use external .obj files for polygons
  - accomodates up to order 36 (includes quadrilateral and triangle faces)
- using vary to move lights
  - requires changes to language
- new primitive shapes
  - requires changes to language
  - new MDL commands (cylinder, cone, pyramid)
