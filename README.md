# YOLO Alert System (Python + OpenCV + YOLOv8)

## Project Description
This project is a real-time object detection alert system built using Python and the YOLOv8 deep learning model.

The program captures video from a webcam and uses the YOLO object detection model to identify objects in each frame. When a specified object (for example a person) is detected, the system triggers an alert and prints a notification in the console.

Detected objects are highlighted with bounding boxes and labels on the video feed, allowing the user to monitor detections in real time.

This project demonstrates how computer vision and deep learning can be used to build simple real-time monitoring and alert systems.

---

## Technologies
- Python
- OpenCV (cv2)
- YOLOv8 (Ultralytics)
- NumPy

---

## How It Works
1. The program loads the YOLOv8 object detection model.
2. The webcam captures live video frames.
3. Each frame is processed by the YOLO model.
4. The model detects objects in the frame.
5. The system filters detections to specific objects (for example **person**).
6. Bounding boxes and labels are drawn around detected objects.
7. If a target object is detected, the system prints an alert and optionally plays a beep sound.
8. A cooldown timer prevents repeated alerts from triggering too frequently.

---

## How to Run

Install the required libraries:

pip install ultralytics  
pip install opencv-python  
pip install numpy  

Run the program:

python main.py

The YOLO model file (**yolov8n.pt**) will be automatically downloaded by the Ultralytics library if it is not already available.

---

## Example Output

The program opens the webcam and displays:

- Bounding boxes around detected objects
- Object labels (person, car, etc.)
- Real-time alerts when a target object is detected

Example console alert:

[ALERT] 12:45:30 -> person x1

---

## Project Purpose

This project demonstrates how YOLO-based object detection can be used to build simple real-time alert systems.

Applications of similar systems include:

- security surveillance
- intrusion detection
- restricted area monitoring
- smart building monitoring
- automated safety systems

---

## Future Improvements

Possible improvements include:

- Detecting multiple object types
- Sending alerts via email or notifications
- Saving detection events to a log file
- Adding a graphical user interface
- Using video files instead of a webcam
- Improving performance with GPU acceleration

---

## Author
Sean Michaeli
