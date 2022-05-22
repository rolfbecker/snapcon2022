# Snap!Con 2022 Conference - HSRW EOLab Contributions 

We use this repo to develop our proposals for the conference: https://www.snapcon.org/conferences/2022/program/proposals/new

## Call for Proposals
We invite participation by current or potential Snap! users, teachers, researchers or developers. Topics:

* Teaching and learning computer science
* Teaching and learning mathematics
* Teaching and learning, period
* Extensions to Snap!
* Attracting independent learners 

For an interactive and interesting conference, we’d love to see more (live) demos and (short) discussions, and fewer slides. We welcome several modes of participation:

* Open-our-eyes Lightning talks (5 min)
* Show us your project (3-5 min)
* Impactful Talks (15 min)
* Powerful Panels (60 min)
* Community-gathering Birds-of-a-Feather sessions (30 min)
* Interactive Workshops (60 min)

If you propose a workshop, we’ll require a detailed agenda showing how you’re going to engage the audience to participate. We can’t wait to see what you’re doing!

## Introduction to EOLab Activities

The Earth Observation Lab [(EOLab)](https://wiki.eolab.de/) team at Rhine-Waal University of Applied Sciences [(HSRW)](http://www.hsrw.eu) is working on computer vision and object recognition for applications in environmental monitoring and conservation. In addition, the EOLab team is also involved in the field of STEM education (K12) by creating open teaching materials and conducting workshops with schools for this purpose.  

A new activity that we find very exciting and promising is teaching the basics of machine learning to young students by combining Snap! and neural network-based object detectors running on backend servers. Objects on webcam snatshots or image files are identfied with convolutional neural networks running in the background. The assigned object labels and bounding boxes can then be used in Snap! programs.  

Snap! is used to take snapshots (still images) from the local webcam. These pictures are transmitted to a backend server running an object detection software. The backend server reports the bounding box, the object type, and the confidence level for each identified object on the image back to Snap! This information is overlaid with the still image in Snap! This object metadata can be used to control Snap! programs such as games. 

For our current development, we mainly use small but powerful NVIDIA Jetson Nano computers as backend running DetectNet to identify objects in images or video streams. 
To achieve this coupling, we installed a Python Flask web server on the NVIDIA Jetson Nano that provides a RESTful API to the DetectNet object detector instance. This backend server process accepts images encoded as base64 strings, transforms them back to a standard image format, and forwards them to the object detector. The result of the object detection is the bounding box, the suspected object type, and the confidence level of the detection.

Several JavaScript blocks in Snap! (the frontend) were designed to connect to the backend server, take a snapshot from the webcam video stream, encode it as a base64 string, send it to the backend server, to receive the response, and to create new sprite with transparent rectangles as costumes representing the identified objects' bounding boxes.   


## Workshop 

[Workshop 1](Workshop_1.md)

## Talk

[Talk 1](Talk_1.md)

## Lightning Talk

[Lightning Talk 1](Lightning_Talk_1.md)

