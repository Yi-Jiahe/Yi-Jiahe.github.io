# Motion Based Multiple Object Tracking
During the summer of my 3rd year, I did an internship with Temasek Laboratories at NUS. During my internship, I worked on developing an algorithm to detect and track mulitple moving objects in a scene, and return their 3D positions in real time.

My first task during the internship was to implement an algorithm tested in MATLAB into Python. To do so, I made use of the OpenCV library and got to know the functionality it provided in terms of image and video processing and methods for extracting useful information from images and videos. I also familiarsed myself with data visualization using a combination of OpenCV and the python plotting library matplotlib.

From there, I also studied photogrammetry concepts such as the direct linear transform (DLT), epipolar geometry and triangulation to determine the 3D position of the 2D detections within the images from the cameras. We used a binocular setup to triangulate the 3D position of objects located within the field of view of both cameras. I also made use of the photogrammetry concepts I had learnt to implement an algorithm that would triangulate the position of any object detected by at least two cameras, regardless of their positions or orientations, so long as they were both able to see the object.

Finally, I also worked on implementing the algorithm in real-time, which involved performing the detections on the video stream from multiple cameras, tracking each object, matching their detections from both cameras and performing the triangulation based on the position and pose of each camera containing the detection.

### [Back to Home](index.md)
