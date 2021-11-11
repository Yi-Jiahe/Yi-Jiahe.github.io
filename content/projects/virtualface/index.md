# Virtual Face

With the increased interest in VR and computer vision leading to a boom in popularity for face tracking applications and promising solutions, I decided to try my hand at it to figure out how such a solution might work.

![Integration](images/Integration.png)

[Virtual Face](https://github.com/Yi-Jiahe/virtual-face) is a combination of a Computer Vision face and body tracking solution using Google's MediaPipe library, and a [renderer](https://github.com/Yi-Jiahe/cv-controller) which makes use of the tracking data, built in Unity.

I made use of the facial landmarks to determine the position and pose of the head, abstracting the required parameters for the renderer. The tracking program also starts a socket server such that applications can connect to it to request for the tracking data.