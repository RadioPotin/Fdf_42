# Fdf_42

Fdf stands for "Fil De Fer" which means "wire". The goal of the project is to create a Wire topographic Map renderer. The program must take a specifically formatted map file that consists in lines of a consistant number of integers separated by space characters. Each integer represents an altitude and this will eventually be used to create a topographical grid.
The goal is to simulate a 3D coordinate system and calculation and print it pixel by pixel on a 2D Screen.
The subject imposes at least two different projections, so I've coded my program to use parallel and isometric projections.

Here the set of features my Fdf has:
1. One static structure pointer as environment that gets modified whenever needed.
2. Matrix calculation, that is for translation, scaling and rotations.
3. An implementation of the Bresenham algorithm for line drawing on screen. 
4. Color management and color gradient based on the Z coordinates of every given point.
5. Zoom in/out.
6. Translation on X and Y.
7. Independant scaling for the Z dimension.
8. A User Interface Chart Legend (Keybindings and important features)

Nota Bene: On the colour coding, I've divided altitudes in 5 based on the highest altitude found in the map.
The 1/5 of the highest altitude will be drawn in blue, the next fifth will be drawn in green, the next in brown, the next in orange and every altitude that come as close as 1/5 of the heighest altitude will be drawn in red. This allows higher readability of the map as well as a nice colour touch

Here are a few screenshots of different sized maps: <br> <br>
![SMALL MAP](https://i.imgur.com/lxn50Xb.png) <br>
Screenshot 1: An example of a small map of heterogenous altitudes. <br> <br>
![MEDIUM MAP](https://i.imgur.com/1LCW3Mx.png) <br>
Screenshot 2: An example of a map of medium size.<br> <br>
![LARGE MAP](https://i.imgur.com/RVBht1a.png) <br>
Screenshot 3: An example of a large map, generated by the Map Generator found here: [42MapGenerator Github](https://github.com/jgigault/42MapGenerator) <br> <br>
All the maps used here (and more) can be found under the ressource/maps/ directory found in the Fdf/ repository.

