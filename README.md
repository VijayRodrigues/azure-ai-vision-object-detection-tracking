# Azure AI Vision – Object Detection and Frame-Based Tracking

## Project Overview

This project demonstrates **object detection and basic object tracking** using **Azure AI Vision through Vision Studio**.  
The experiment evaluates how Azure AI detects objects within images and how detection results can be compared across video frames to observe movement within a scene.

The project was conducted using workspace images and a short video recording of a home office environment.

---

## Objectives

The main objectives of this experiment were:

- Explore object detection capabilities using Azure AI Vision
- Analyze how the system identifies objects within different images
- Observe how detected objects change position across sequential video frames
- Evaluate detection accuracy using bounding boxes and confidence scores

---

## Technologies Used

- Microsoft Azure AI Vision
- Azure Vision Studio
- Computer Vision models
- Image analysis
- Video frame analysis

---

## Experiment Description

### Image Object Detection

Three different workspace images were analyzed using Azure AI Vision.  
The system automatically detected objects present in the scene and generated **bounding boxes** around them.

Detected objects included:

- Person
- Chair
- Monitor / Display
- Keyboard
- Table
- Plant

The system also provided **confidence scores** indicating the probability of correct detection.

---

### Object Tracking Using Video Frames

To demonstrate object tracking, a short video of a workspace environment was recorded.  
In the video:

- A person enters the frame
- Sits at the workstation
- Waves at the camera

Three frames were extracted from the video and analyzed using Azure AI Vision.  
By comparing detection outputs across these frames, the movement of the detected person can be observed through changes in the bounding box position.

Although Vision Studio performs object detection on individual images, analyzing multiple frames allows a simple observation of object movement across time.

---

## Repository Structure

```
report/
SIG788_Task5_Object_Detection_Tracking_Azure_AI_Vision.pdf

images/
workspace_image_1.jpg
workspace_image_2.jpg
workspace_image_3.jpg

results/
detection_result_1.png
detection_result_2.png
detection_result_3.png

video/
workspace_tracking_video.mp4
azure_ai_detection_demo.mp4
```




---

## Example Detection Output

Example object detection results generated using Azure AI Vision.

![Detection Example](results/detection_result_1.png)

---

## Key Observations

- Azure AI Vision successfully detected common objects within workspace environments.
- Bounding boxes and confidence scores helped evaluate detection accuracy.
- In some cases, the system classified a computer monitor as a **television**, showing how models group visually similar objects.
- Sequential frame analysis allowed simple observation of movement across video frames.

---

## Conclusion

This experiment demonstrates how Azure AI Vision can be used to implement object detection and analyze visual scenes using cloud-based computer vision services.

The results show that Azure AI Vision is effective for identifying common objects and can support real-world applications such as automation, surveillance, and workspace monitoring.

---

## Author

**Vijay Rodrigues**  
Project created as part of experimentation with Azure AI Vision and computer vision concepts.
