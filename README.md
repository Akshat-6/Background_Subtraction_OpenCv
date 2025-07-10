# Background_Subtraction_OpenCv
Implementation of background subtraction using OpenCV to detect motion and foreground objects in videos and image sequences.


🕵️ Background Subtraction using OpenCV


This project implements background subtraction, a fundamental technique in computer vision used to detect moving objects or extract foreground elements from video streams and image sequences. 
 The implementation utilizes OpenCV’s built-in background subtraction models for dynamic and real-time applications.

🎯 Objective


To extract the foreground (moving objects) from a static background using frame-wise analysis and background modeling techniques. This is commonly used in:


Motion detection

Object tracking

Surveillance systems

Human activity recognition


📂 What’s Implemented

✅ 1. Background Subtraction Using cv2.createBackgroundSubtractorMOG2()

Gaussian Mixture-based Background/Foreground Segmentation

Supports shadow detection and learning rate tuning


✅ 2. Optional: cv2.createBackgroundSubtractorKNN()

K-Nearest Neighbors based background model

More accurate for dynamic backgrounds


✅ 3. Real-Time Video Feed Support

Can be applied to:

Video files (e.g., .mp4)

Webcam streams (cv2.VideoCapture(0))


✅ 4. Foreground Mask Visualization

Binary mask showing moving objects

Optional contour detection and bounding box drawing


📁 Project Structure


background-subtraction-opencv/
├── background_subtraction_mog2.py         # Main background subtractor script
├── input_video.mp4                        # (Optional) Video file for testing
├── sample_frames/                         # Output frames with foreground mask
├── README.md
└── requirements.txt




💻 Technologies Used

Python

OpenCV (cv2)

NumPy

Matplotlib (optional for frame display)


🚀 How to Run

1.Clone the repository:


git clone https://github.com/yourusername/background-subtraction-opencv
cd background-subtraction-opencv


2.Install dependencies:


pip install opencv-python numpy


3.Run the script:


python background_subtraction_mog2.py


Replace cv2.VideoCapture() path if testing on a video file or camera stream.



📊 Sample Output


Binary mask highlighting moving/foreground objects

Real-time update of original frame vs extracted mask

Optionally draw bounding boxes around detected motion



🌟 Applications


CCTV surveillance

Traffic monitoring

Sports player tracking

Gesture recognition


🧠 Additional Insights

MOG2 is more adaptive and supports shadow detection

KNN performs better with moving backgrounds but is slower
