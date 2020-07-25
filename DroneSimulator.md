# Drone Simulator
Orignally the project started out as a drone and physics simulator in Python. I started by simulating various aspects of a quadcopter, such as how an input voltage would drive the propellers, creating a thrust and torque, which would be applied to the quadcopter. To perform the simulation, I also had to write a physics simulation, building an update loop, gravity and ground collisions, alongside a visualisation and user interface. As I was tuning the altitude hold controller, I took a break and decided to make the switch to Unity.

<img src="/images/QuadcopterPython.png"
	width="500"/>

The visualization and user interface were extremely crude in python, and was only implemented in the xy-plane. As I wanted to focus more on the dynamics and control systems behind the drone, I decided it would be best to switch to a solution with a pre-built physics and rending engine. I also had plans to learn Unity and its scripting language C#, so I decided it would be a good opportunity to do so.

<img src="/images/QuadcopterUnity.png"
	width="750"/>

It was slow going as I learnt the ropes of Unity, its objects and properties, as picking up the syntax of C#, which made me appreciate the numerical libraries and the understanding I had of the simulation I had built in Python. Eventually though, I managed to model the individual rotors and how an input from the controller would cause a net force and torque to be generated on the quadcopter. It was at this point that I really began to see the advantages of a 3rd party solution such as Unity.

### [Back to Home](index.md)