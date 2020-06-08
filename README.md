# Final Project Proposal
Peihua Huang and Jackie Lin (pd 10)

## Features
We will be implementing the following features in our project:
- light
    ```
    light lightname r g b x y z //creates a light with rgb values r, g, b at (x, y, z)
    light lightname r g b x y z [knob] [x_axis] [y_axis] [z_axis] //creates a moving light that starts moving from (x, y, z)
    //if any of the axis is set to 0, the light will not move on that axis, if it's set to 1, the light will move
    ```
  - existing MDL command
  - will add light to symbol table
  - all lights will be used in calculating diffuse and specular reflection
- mesh
    ```
    mesh [constants] :filename //rendeers a mesh or set of edges from an OBJ file
    ```
  - existing MDL command
  - will parse external .obj files (v and f commands) for polygons
  - accomodates up to order 36 (includes quadrilateral and triangle faces)
- using vary to move lights
  - requires changes to language
- new primitive shapes
    ```
    cylinder [constants] x y z r h //renders a cylinder whose center (top cap) is (x, y, z) with radius r and height h
    cone [constants] x y z r h //renders a cone whose center (base) is (x, y, z) with radius r and height h
    pyramid [constants] x y z w h //renders a square pyramid whose apex is (x, y, z) with width w and height h
    ```
  - requires changes to language
  - new MDL commands (cylinder, cone, pyramid)
