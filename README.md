# Document for "Automated Vehicle Detection and Parking Management System"

### Table of contents
- 1 Purpose
- 2 Introduction to Our Test
- 3 Content of Files Above

## 1 Purpose
The purpose of this automated vehicle detection and parking management system is to enhance the efficiency of parking space utilization and streamline vehicular monitoring. This system significantly contributes to the reduction of traffic congestion in parking areas and improves the overall user experience in locating available parking spots. By employing advanced computer vision and machine learning techniques, the system provides real-time information on parking space occupancy, thereby aiding in effective parking space management. This technology is crucial for urban areas, shopping centers, and public facilities, where parking space optimization is essential.

## 2 Introduction to Our Test
Our test involves deploying an automated system that utilizes video surveillance to monitor and manage parking spaces. The system is designed to identify vehicles using the YOLO (You Only Look Once) object detection model and to monitor the occupancy of parking spaces within a video frame. This test is conducted to evaluate the system's accuracy in detecting vehicles and its efficiency in calculating the number of available parking slots. The test provides insights into the system's applicability in real-world scenarios, highlighting its potential to enhance parking management and traffic flow within congested areas.

## 3 Content of Files
- [detect.py](https://github.com/Kane-Nguyen/Parking-Slot-Detection-Document/blob/main/detect.py): This script is the core of the vehicle detection and parking space monitoring system. It processes video footage, detects vehicles using the YOLOv8x model, and identifies occupied parking spaces. The script also visually displays the total and available parking slots on the video feed, providing real-time parking space information.
- [polyline.py](https://github.com/Kane-Nguyen/Parking-Slot-Detection-Document/blob/main/polyline.py): This auxiliary script is used for the initial setup of the parking monitoring system. It enables users to manually define parking areas in a video by drawing polylines. These polylines, along with their respective area names, are saved and utilized by the [detect.py](https://github.com/Kane-Nguyen/Parking-Slot-Detection-Document/blob/main/detect.py) script for monitoring the predefined parking spaces. This tool is essential for customizing the system to specific parking layouts.
- `coco.txt`: A text file containing a list of object classes that the YOLO model can detect. This file is crucial for the [detect.py](https://github.com/Kane-Nguyen/Parking-Slot-Detection-Document/blob/main/detect.py) script to identify specific object types, such as vehicles, within the video frames.
- `03.mp4`: The video file used for testing the system. It provides the visual data needed for vehicle detection and parking space monitoring.
- `03`: A data file used by both scripts, containing information about the drawn polylines and area names. This file ensures that the parking areas are consistently recognized and monitored across both scripts.
