# openGL_motiondetection
Max/MSP/Jitter primarily openGL-based motion tracking and triangulation

This patch takes 2 2D video sources and triangulates movement between them to determine the actual position of objects in 3D space.  

This project is primarily designed for tracking the movement of dancers in a normalized spaced.

Normalization for this purpose is a high level of contrast between the object(s) to be tracked and the background. Cameras should be positioned at right angles from each over.

Mode 1: Triangulate 3D position based on 2 2D inputs
Mode 2: Determine the 2D position of motion on 1 2D input
Mode 3: Determine the 2D position of motion on 2 independent 2D inputs


Future additions:
1)Distrort the video input textures (or output textures) to accurately map video projection output.
2)Further optimise the centroids section to be openGL based.
3) Determine the angle of each camera, and adjust accordingly, to accurately map non-right angled spaces.
