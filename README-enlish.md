# PSP-MP brief introduction
PSP-MP, a subway platform passenger standing position dataset created using Blender software. The dataset includes 200 test scenarios. The IMG directory stores binocular images of the subway platform layer, with a single image resolution of 1280 * 720Pixel and a JPG format. The GT directory stores information such as the standing position, height, and orientation of passengers on the platform layer in the platform coordinate system.

# Sample dataset
Binocular image of scene 112
![Binocular image](https://github.com/yanconggit/PSP-MP/blob/main/IMG/IMG_112.jpg)
Scene 112: Real Standing Position Display of Passengers
![The standing position of passengers and the projection position of binocular cameras on the platform](https://github.com/yanconggit/PSP-MP/blob/main/markdown/%E7%9C%9F%E5%AE%9E%E5%80%BC%E5%9D%90%E6%A0%87.jpg)

# Binocular camera parameters
Stereoscopic model: Parallel

Baseline distance: 200mm

Lens focal length: 40mm

The coordinates of the binocular camera in the platform coordinate system (1.3, 8.0, 3.0), with a depression angle of 10°

# Rules for establishing platform coordinate system
The origin of the platform spatial coordinate system is taken as the point where the end door at the end wall in the following direction intersects with the platform screen door parallel to the track and the ground. The Y-axis direction is taken as the positive direction of the platform spatial coordinate system, and the direction perpendicular to the fixed platform screen door facing the platform is taken as the positive X-axis direction. The unit length is taken as one meter to obtain the platform spatial coordinate system.

# GT csv introduction
| Symbol | meaning |
| ---- |---- |
| X | The coordinate value of the passenger's standing position on the X-axis of the platform coordinate system |
| Y | The coordinate value of the passenger's standing position on the Y-axis of the platform coordinate system |
| H | Passenger's height information |
| RZ | Passenger's facial orientation information |
