# Face Detection and Attendance System

cv2.imshow('Webcam',img)
<img width="483" alt="image" src="https://github.com/user-attachments/assets/6dba32e6-d152-4788-9229-e2e999582fa6">
<img width="483" alt="image" src="https://github.com/user-attachments/assets/16f8e9ce-88ef-4727-9a4a-d11c8ec4a799">

## Project Overview
This project implements a real-time face detection and attendance system using Python, OpenCV, and the face_recognition library. The system captures live video feed from a webcam, detects faces, and matches them against a set of pre-stored images to record attendance.

## Images Used
The system uses images of well-known personalities for demonstration purposes:

Bill Gates
Jack Ma
Elon Musk
These images are stored in the ImagesAttendance folder and are used as the reference images for face detection and recognition.

## How It Works
- Image Encoding:
    - The program reads images from the ImagesAttendance folder and converts them into encodings using the face_recognition library. These encodings represent the unique features of each face.
- Face Detection:
    - The system captures video feed from the webcam.
    - Each frame is resized and converted to RGB format.
    - The program detects faces in the current frame and compares them with the known encodings.
- Face Recognition:
    - The system calculates the distance between the detected face and all known encodings.
    - The face with the smallest distance (i.e., the closest match) is recognized.
    - If a match is found, the person’s name is displayed on the screen, and their attendance is marked in the Attendance.csv file with the current time.
## Requirements
Python 3.x
OpenCV
face_recognition
Numpy
A webcam for capturing the video feed
The webcam will start, and the system will begin detecting faces.
If a recognized face is detected, the name will be displayed on the screen, and the attendance will be recorded.
## Output
Attendance is logged in a CSV file named Attendance.csv, with the name of the recognized individual and the time of recognition.
