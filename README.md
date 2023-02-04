# BlackWings Hackathon 2023
DigitalDiva: Elevating Education

## Inspiration
We were inspired by the increasing use of online meeting platforms like Zoom, Google Meet, Teams used to facilitate classroom learning. For students and teachers that are present in Zoom, attendance plays a big role in encouraging students to come to class and actively participate in lessons. Our objective for DigitalDiva, in brief, is to facilitate a smooth day-to-day life routine, and this implementation will eradicate the possibility of human error, promote timesaving, and eliminate the need for proxy attendance.

## What it does
DigitalDiva is an automatic attendance management system. By using Face Recognition technology, we were able to make a portable device for managing the students’ attendance. First, students are encouraged to take a picture of themselves to add into our dataset. Our algorithm is then able to identify everyone using a square overlay with their name on the bottom while noting down (name, time) in an Attendance_ninjas.csv file.

## How we built it
We built it using the facial recognition libraries such as Cmake, Dlib, Facial_recognition, ImageGrab, PIL, and Opencv. The facial recognition library only needs one image to detect the face. As the face encodings are pre-defined, we append it into a list in our dataset. We incorporated the compare feature to test our accuracy and return the distance value from the given training image.  The ImageGrab from the PIL function helps to capture the computer screen, where we tell it to capture the screen which is our online meeting every 1ms. As this is being captures, to make sure the application is detecting faces we programmed in to include bounding boxes with names for faces detected by the system and then note them down in a CSV file, as Name in one column and Time (24:00 hour format) in another.

## Challenges we ran into
Some challenges we ran into was how the screen sharing feature on Zoom and Teams created conflict in using the software. However, we noticed that a lot of instructors tend to take screenshots of their meeting screen for attendance a few minutes after class started. We applied the same strategy as potential teachers and the software worked as intended.

##OutPut
