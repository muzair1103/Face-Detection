##Video Face Detection using DeepFace and OpenCV
This script performs face detection on a video using the DeepFace library and OpenCV. It extracts faces from each frame of the input video, draws bounding boxes around the detected faces, and saves the processed video with bounding boxes as output.

Requirements
Python 3.10
opencv-python 4.8.0.76
deepface 0.0.89

Installation
Install Python 3.x from python.org.
Install OpenCV and DeepFace library using pip:
pip install opencv-python-headless
pip install deepface

Usage
Ensure that your input video is located in your Google Drive and update the num variable to specify the video number.
Run the script. It will process the video, detect faces using the RetinaFace detector, draw bounding boxes around the detected faces, and save the processed video with bounding boxes.
The output video will be saved to your Google Drive with the filename retinafaceop{num}.mp4.

Script Details
The script loads the input video specified by the num variable.
It reads each frame of the video and performs face extraction using the RetinaFace detector from the DeepFace library.
Bounding boxes are drawn around the detected faces on each frame.
The processed frames with bounding boxes are written to an output video file.
Progress is printed indicating the number of frames processed.
Once processing is complete, the input and output video files are released, and OpenCV windows are closed.

References
DeepFace GitHub Repository
OpenCV Documentation
Python Documentation

For more details on the DeepFace library and its capabilities, please refer to the official documentation.
