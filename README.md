# Air_Canvas_ml_model

Ever wished to capture your imagination by just waving your finger in the air? In this post, we have an Air Canvas that can draw anything on it by simply moving our hands and observing the landmark on the hand knuckles. A virtual drawing tool (Computer vision project) that allows you to draw in the air using hand gestures, thanks to the powerful combination of OpenCV and MediaPipe.

### 🔧 Tools and Libraries Used:

- **Python3:** The primary programming language used for this project. 
- **NumPy:** A library for efficient numerical computation, used for array and matrix operations.

- **OpenCV:** This open-source library is essential for real-time computer vision tasks. It helped me capture and process video frames from the webcam seamlessly.

- **MediaPipe:** Developed by Google, MediaPipe is a fantastic framework for building multimodal machine learning pipelines. In this project, I used MediaPipe for hand tracking, enabling accurate and real-time recognition of hand landmarks.

### How It Works:
- Capture Video: Using OpenCV, the script captures live video feed from the webcam.
- Process Frames: Each frame is processed using MediaPipe to detect and track hand landmarks.
- Draw Landmarks: The detected hand landmarks are drawn on the video frames, creating a virtual canvas for drawing in the air.

  
### Algorithm
1. Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)

2. Prepare the canvas frame and put the respective ink buttons on it.

3. Adjust the values of the mediapipe utilization to detect one hand only.

4. Detect the landmarks by passing the RGB frame to the mediapipe hand detector.

5. Detect the landmarks, find the forefinger coordinates and keep storing them in the array for successive frames.(Arrays for drawing points on canvas)

6. Finally, draw the points stored in an array on the frames and canvas.

<img width="949" alt="image" src="https://github.com/kanishkasah20/Air_Canvas_ml_model/assets/114860158/77a756ac-54ad-49c2-b784-c46ee868a01d">

