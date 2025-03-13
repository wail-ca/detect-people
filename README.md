# Person Detection using YOLOv3

**Overview**

This project implements real-time person detection using YOLOv3 and OpenCV. It processes video frames, detects people using a pre-trained YOLOv3 model, and highlights them with bounding boxes. The system can work with both video files and live webcam feeds.

Requirements

Before running the project, install the necessary dependencies:
```
pip install opencv-python numpy
```
Additionally, download the YOLOv3 model files:

yolov3.weights
yolov3.cfg
coco.names

Place these files in the project directory.

**Usage**

# 1. Clone the repository

```
git clone https://github.com/wail-ca/detect-people.git
```
```
cd person-detection-yolo
```
# 2. Run the script
```
python detect_people.py
```
-To use a video file, replace "video.mp4" in the script with your file name.

-To use a webcam, replace "video.mp4" with 0.

# 3. Exit the program
Press q to stop detection and close the window.
How It Works

•Loads YOLOv3 model and class labels from the COCO dataset.

•Processes each frame from the video or webcam.

•Identifies objects and filters for people (class_id = 0).

•Uses Non-Maximum Suppression (NMS) to reduce redundant bounding boxes.

•Draws bounding boxes around detected people.


# Example Output

A sample output showing detected people in a video stream:

 (Replace with your own image)

**License**

This project is for educational and research purposes only.
copyright to Wail ©
