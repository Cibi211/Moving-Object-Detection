**Motion Detection Using OpenCV and Python**

This project is a basic motion detection program built with Python, OpenCV, and imutils. It uses a webcam to capture video frames and detects movement by comparing the first frame with subsequent ones. When motion is detected, the program highlights the moving object with a bounding box and updates the status on the screen.

**Features**

Captures live video using the webcam.
Converts video frames to grayscale and applies Gaussian blur for better motion detection.
Detects and highlights moving objects by comparing the current frame with the first captured frame.
Displays the motion status ("Normal" or "Object moving") on the video feed.
Allows the user to stop the program by pressing the "p" key.

**How It Works**

Capture the First Frame: The program captures the first frame of the video as a reference for motion detection.
Preprocessing: Each frame is resized, converted to grayscale, and blurred to reduce noise.
Frame Differencing: The absolute difference between the first frame and the current frame is calculated to identify changes.
Thresholding and Contours: Thresholding is applied to highlight significant changes, and contours are detected to identify moving objects.
Drawing Bounding Boxes: For detected objects larger than a predefined area, a bounding box is drawn around the object on the video feed.
