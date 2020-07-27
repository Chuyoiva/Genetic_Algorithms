# Genetic_Algorithms
Genetic Algorithms applied on a Unity3D project to create autonomous agents which navigate a virtual environment.

Each individual contain the following genes:

-A Vector3 which determines the direction of movement of the individual. X and Z values go from -1f to 1f using Random.Range(). Y value is always 0.
-A movement speed which determines how fast the individual will move in a certain direction. Goes from 0f to 2f.
-A movement time which determines how long will the individual will move in a certain direction. Goes from 0.5f to 3f.

The algorithm evaluate the performance of individuals navigating their environment using the following fitness method:

Fitness=1-(d/D)+((speed)/ 200)+((Time) / 300)

In which:
-D = The distance between the origin point and the destination point.
-d = The distance between the individual's last position and the destination point.
-speed = The average of all the individual's movement's speed.
-Time = The average of all the individual's movement's time. 

![Settings_screen](https://i.imgur.com/a5gv6Oh.png)
![Level 1](https://i.imgur.com/UhwyK1I.png)
![Level 2](https://i.imgur.com/INM6ELd.png)
![Level 3](https://i.imgur.com/PA5P9ZT.png?1)
