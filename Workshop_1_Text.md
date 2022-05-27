# Workshop 1:<br>Object Detection in Snap! with DetectNet on NVIDIA Jetson Nano

## Other Helpers for Participants during the Activity
Harley Lara, Ali Farzizada, Ilgar Rasulov

## Significance and Relevance of the Topic

Artificial intelligence is a prevailing technology that poses opportunities and risks for society and the environment. Building knowledge and skills in schools is critical to enable students early on to master the technology in stead of being mastered, to demystify AI, to acquire critical reflection competencies, to assess the opportunities and limitations of AI for problem solving.
The usability of many AI toolkits continues to improve. Less and less expert knowledge is required to use them. 

This Simplification can be further advanced. We use SNAP! to communicate with object detectors based on convolutional neural networks (CNN). In the current setup we utilize to the object detection software DetectNet running on a NVIDIA Jetson Nano embedded computer as backend server.

Snap! is used to take snapshots (still images) from the local user PC webcam. These pictures are transmitted to the DetectNet server. This backend object detector reports the bounding box, the object type, and the confidence level for each identified object on the image back to Snap! This information is overlaid with the still image in Snap! This object metadata can be used to control Snap! programs such as games.


## Rough Agenda for the Workshop

In this practial workshop we learn how to use convolutional neural network (CNN) based object detectors in SNAP! The reported object information can then be used for control in SNAP! programs such as games. 

The workshop is provided in a mixed format: on-site as well as remote! 

The object detector software DetectNet is running on NVIDIA Jetson Nano computers, which we will provide in a Virtual Private Network (VPN). The credentials to access the network will be shared to the registered participants.

Each NVIDIA Jetson Nano computer can currently serve only one user PC/laptop. Therefore, **we need to limit the number of connected user computers to 10**. We suggest working in groups of 2 with one computer so that 20 people can participate. 

### Schedule / Preparation

* Introductory presentation and system setup (15 minutes)
* Interactive workshop (30 minutes)
* Discussion / reflection (15 minutes)

The workshop will be held on-site in Heidelberg. We will set up a virtual private network (VPN) such that people can connect remotely. Since our computing rescources are limited interested participants must register for the workshop. The credentials for the VPN will be shared after successful registration.

## Expected Audience

Technically interested teachers, trainers and other people who want to experience and assess the use of AI for computer vision in SNAP! Users without a deep tech background are welcome but our draft training material is still beta and nerdy. Patience is required :-)

## Participant Equipment Requirements

* All participants need SNAP! on their computer.
* All participants need a webcam accessible from SNAP!
* On-site participants will need laptops with WiFi to connect to the local private network we set up.
* Remote participants will need to install OpenVPN client software to connect to our private network.

## Other Critical Information

**To the organizers on-site:**
- We bring 10 preinstalled NVIDIA Jetson Nano computers equipped with wifi interfaces to the workshop location. 
- We also bring a VPN enabled WiFi router which provides its own local private WiFi network, aka "workshop network". This WiFI router itself is a VPN client to our external VPN server. The NVIDIA Jetson computers as well as the local participants' computers will connect to the workshop network through WiFi. 
- Remote users have to install OpenVPN and connect to the VPN server in order to join the workshop network. The workshop router handles the traffic between user computers (local or remote) running SNAP! and the NVIDIA Jetson Nano computers running DetectNet. 
- It is a **strict requirement** that our **workshop router** gets an **internet connection** (via wifi or ethernet) on the workshop location by the local organizers.
- We have to establish a procedure for workshop registration to limit the number of participants (because of limited hardware resources)

l
