# Drone Simulator
Orignally the project started out as a drone and physics simulator in Python. I started by simulating various aspects of a quadcopter, such as how an input voltage would drive the propellers, creating a thrust and torque, which would be applied to the quadcopter. To perform the simulation, I also had to write a physics simulation, building an update loop, gravity and ground collisions, alongside a visualisation and user interface. As I was tuning the altitude hold controller, I took a break and decided to make the switch to Unity.

![Python](\assets\images\dronesimulator\QuadcopterPython.png)

The visualization and user interface were extremely crude in python, and was only implemented in the xy-plane. As I wanted to focus more on the dynamics and control systems behind the drone, I decided it would be best to switch to a solution with a pre-built physics and rending engine. I also had plans to learn Unity and its scripting language C#, so I decided it would be a good opportunity to do so.

![Unity](\assets\images\dronesimulator\QuadcopterUnity.png)

It was slow going as I learnt the ropes of Unity, its objects and properties, as picking up the syntax of C#, which made me appreciate the numerical libraries and the understanding I had of the simulation I had built in Python. Eventually though, I managed to model the individual rotors and how an input from the controller would cause a net force and torque to be generated on the quadcopter. It was at this point that I really began to see the advantages of a 3rd party solution such as Unity.

<!-- blank line -->
<figure class="video_container">
  <video controls="true" allowfullscreen="true">
    <source src="/assets/videos/simulated_drone_flight.mp4" type="video/mp4">
  </video>
</figure>
<!-- blank line -->

The simulation broke down the drone into its various components, such as the rotors, main body, flight controller and sensors. The rotors generated a force and a torque based on its speed, determined by its intrinsic parameters as well as the throttle input from the flight controller. The flight controller supports mutltiple flight modes, which translate input controls into throttle commands. It includes a stabilized flight mode, which uses sensor data and PID controllers to adjust the throttles automatically based on the motor mixing algorithm. Each sensor has its own module, which simulates how the actual sensor works and returns measurements similar to the real sensor. The flight controller can choose which sensors to use and process them such as using an IMU to combine gyroscope and accelerometer readings to find the position and orientation of the body (on which the sensors are mounted). This can be combined with the altimeter data to get a better estimate of the height.

### [Back to Home](/)