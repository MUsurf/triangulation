# Triangulation

The purpose of this function is to find the distance using 2 cameras.


## Camera Setup
Put 2 cameras a set distance apart and facing the same direction
These cameras should be able to detect the object
Each camera extracts an X degree and a Y degree angle of the object relative to the camera

## How it works
Input the the X and Y angle of each camera:

((int cam1X), (int cam1Y), (int cam2X), (int cam2Y))

The function gets the x distance and the y distance the object *relative to Camera one*
Then, it finds the total distance using the pythagorean therom.
It then returns the distance of camera one to the object *relative ot the distnace the cameras are apart*

## Why it is important
Some of the most important things the sub does revolves around object interactions. Some of these tasks involve picking up objects, going through gates, and identifying objects. In order to best perform these tasks, the sub needs to know how far it is from these objects. This is why the "triangulate" function is important. With a total of 4 cameras on the sub, this function should allow us to find the distance of any object on 2 sides of the sub.
