Video Face Detection using DeepFace and OpenCV
This script performs face detection on a video using the DeepFace library and OpenCV. It extracts faces from each frame of the input video, draws bounding boxes around the detected faces, and saves the processed video with bounding boxes as output.

Requirements
Python 3.x
OpenCV (cv2)
DeepFace library


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



Face Recognition and Extraction
This notebook provides functionality for both face recognition and extraction from video files using the DeepFace library. It includes sections for extracting faces from videos, recognizing faces using a pre-built face database, and drawing bounding boxes around detected faces.

Requirements
Python 3.x
DeepFace 0.0.89
OpenCV-Python 4.8.0.76


Installation
You can install the required Python packages using pip:
pip install deepface==0.0.89 opencv-python==4.8.0.76


Usage
Face Extraction from Videos: Follow the instructions in the notebook to extract faces from a video file. You need to specify the input video file path, output directory path to save the extracted faces, and other parameters such as the target duration (in seconds) and frame rate.

Face Recognition: The notebook also includes functionality for recognizing faces in a video using a pre-built face database. This section loads a face database from a text file, compares faces in the video with the faces in the database, and draws bounding boxes around recognized faces.


Face Database
The face database is stored in a text file in the following format:
Face ID: 1, Path: /path/to/face_1.jpg
Face ID: 2, Path: /path/to/face_2.jpg
...
Each line contains the face ID and the path to the corresponding face image.
