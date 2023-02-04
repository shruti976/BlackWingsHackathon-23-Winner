# BlackWings Hackathon 2023
## Title: DigitalDiva: Elevating Education

## Inspiration
We were inspired by the increasing use of online meeting platforms like Zoom, Google Meet, Teams used to facilitate classroom learning. For students and teachers that are present in Zoom, attendance plays a big role in encouraging students to come to class and actively participate in lessons. Our objective for DigitalDiva, in brief, is to facilitate a smooth day-to-day life routine, and this implementation will eradicate the possibility of human error, promote timesaving, and eliminate the need for proxy attendance.

## What it does
DigitalDiva is an automatic attendance management system. By using Face Recognition technology, we were able to make a portable device for managing the students’ attendance. First, students are encouraged to take a picture of themselves to add into our dataset. Our algorithm is then able to identify everyone using a square overlay with their name on the bottom while noting down (name, time) in an Attendance_ninjas.csv file.

## How we built it
We built it using the facial recognition libraries such as Cmake, Dlib, Facial_recognition, ImageGrab, PIL, and Opencv. The facial recognition library only needs one image to detect the face. As the face encodings are pre-defined, we append it into a list in our dataset. We incorporated the compare feature to test our accuracy and return the distance value from the given training image.  The ImageGrab from the PIL function helps to capture the computer screen, where we tell it to capture the screen which is our online meeting every 1ms. As this is being captures, to make sure the application is detecting faces we programmed in to include bounding boxes with names for faces detected by the system and then note them down in a CSV file, as Name in one column and Time (24:00 hour format) in another.

## Challenges we ran into
Some challenges we ran into was how the screen sharing feature on Zoom and Teams created conflict in using the software. However, we noticed that a lot of instructors tend to take screenshots of their meeting screen for attendance a few minutes after class started. We applied the same strategy as potential teachers and the software worked as intended.

## Output

# Initial Meeting
<img width="1377" alt="Screen Shot 2023-02-04 at 1 09 19 PM" src="https://user-images.githubusercontent.com/54175576/216791774-65428caa-4148-4c39-8cb1-6f43fabbf9a4.png">

# Webcam caputring screen every 1ms

<img width="689" alt="Webcam_capture" src="https://user-images.githubusercontent.com/54175576/216791820-25f3ade4-6d5a-44df-9dde-10a02259a322.png">

# Application recognizing participant faces

<img width="684" alt="face_boundings_2" src="https://user-images.githubusercontent.com/54175576/216791835-47f995b3-e43d-4a80-b178-6fc244fbf2eb.png">

<img width="690" alt="face_boundings" src="https://user-images.githubusercontent.com/54175576/216791838-da975ae1-67a1-46a0-bd42-9cb2579873df.png">

# Attendance recorded in CSV
<img width="187" alt="csv_ss" src="https://user-images.githubusercontent.com/54175576/216791855-374cdb10-09d4-4dde-bb4e-19aa8d887d97.png">



