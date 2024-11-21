Marching Cubes

Brief Description:
- This program implements the marching cubes algorithm to generate and render a triangle mesh of an arbitrary scalar field (functions). The resulting mesh is saved to a PLY file. 
- Additionally, the program includes spherical camera manipulation, rendering a box around the marching volume, drawing coordinate axes, and applying lighting effects.

Features:
- Marching Cubes Algorithm: The program executes the marching cubes algorithm on an arbitrary scalar field defined by the user.
- Shader with Lighting: A Phong-like shader is implemented, incorporating ambient, diffuse, and specular lighting effects.
- Camera Manipulation: Allows "click and drag" movement to simulate the object rotating around the origin using spherical coordinates.
- Vertex and Normal Computation: Functions to compute vertex normals and write triangle mesh data to a file are included.
- Rendering: Draws a box around the marching volume and three coordinate axes. The resulting mesh is rendered using VBOs and a VAO alongside glDrawArrays.
- Continuous Mesh Growth: The triangle mesh is rendered during the marching algorithm, creating an animation effect as the mesh grows continuously.

Instructions for Compiling: (Windows System)
- Launch CodeBlocks with all the libraries installed (this include glfw, glew, glm, opengl, glut)
- Open Setting > Compiler, and set the linker to -lfreeglut -lglfw3 -lglew32 -lopengl32
- Create a new project: go to File > New > Project
- On the window pops up, click on Console Application, then click Go
- Continue by clicking on Next and enter a project title, then click on Next and Finish
- In the source folder, copy and replace the main.cpp file with the cpp file I have submitted.
- Click on Build and Run, and the program should successfully run