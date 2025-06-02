# face_detection

👤 Real-Time Face Detection with OpenCV
This project demonstrates real-time face detection using a webcam and OpenCV’s pre-trained Haar Cascade classifier.

📸 Features
Detects human faces from webcam feed

Uses OpenCV’s built-in Haar cascade classifier

Displays a live video window with face detection rectangles

Press q to quit the video stream

🛠 Requirements
Before running the script, make sure you have the following installed:

Python 3.x

OpenCV (cv2)

📦 Install dependencies
bash
Copy
Edit
pip install opencv-python
Note: If you encounter issues with the webcam or GUI, you may also need to install:

bash
Copy
Edit
pip install opencv-python-headless
▶️ How to Run
Save the script (e.g., as face_detect.py)

Run the script in your terminal or IDE:

bash
Copy
Edit
python face_detect.py
A window will open showing your webcam feed.

Detected faces will be highlighted with a green rectangle.

Press q to close the window and exit.

📂 How It Works
Loads OpenCV's pre-trained Haar cascade XML file for frontal face detection.

Captures frames from your webcam.

Converts each frame to grayscale (required for Haar cascades).

Detects faces using detectMultiScale().

Draws a green rectangle around each detected face.

Continuously displays the video in a window until you press q.

📁 File Structure
plaintext
Copy
Edit
face_detect.py
README.md
The cascade file is accessed internally from OpenCV’s data folder:

python
Copy
Edit
cv2.data.haarcascades + "haarcascade_frontalface_default.xml"
🔧 Troubleshooting
❌ Camera not opening?

Make sure no other application is using the webcam.

Try changing the camera index: cv2.VideoCapture(1) or higher.

❌ No face detected?

Ensure there’s enough lighting.

Position your face directly in front of the camera.

🧠 Learn More
OpenCV Haar Cascades Documentation

OpenCV Python Tutorials

📃 License
This project is open source and free to use under the MIT License.
