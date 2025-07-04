# Object detection using NVIDIA Deepstream
This repository contains step-by-step instructions on how to run NVIDIA Deepstream for object detection on video stream, implemented on NVIDIA Jetbot.
<br>
<br>
## Demo
![Demo](Demo.gif)

## Instructions
1. To log in to your Jetson terminal from remote host, use
   ```bash
   ssh <username>@<jetson_ip_address>
   
2. Pull the deepstream container image from NGC catalog according to the version of your Jetson.
   ```bash
   sudo docker pull nvcr.io/nvidia/deepstream-l4t:<version>
   
3. You'll be able to see the deepstream image by running
   ```bash
   sudo docker images

4. Run the deepstream container using
   ```bash
   sudo docker run -it –rm –runtime=nvidia –network host -v <host_directory>:<container_directory> nvcr.io/nvidia/deepstream-l4t:<version>

5. Download an object detection model from [TensorFlow Object Detection Zoo](https://example.com)

   
