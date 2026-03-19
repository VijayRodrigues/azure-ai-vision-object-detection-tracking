# Azure AI Vision – Object Detection and Frame-Based Tracking

## Project Overview

This project demonstrates object detection and basic object tracking using **Microsoft Azure AI Vision through Vision Studio**.

The experiment evaluates how Azure AI Vision detects objects in images and how detection results can be compared across video frames to observe movement within a scene.

The analysis was performed using several workspace images and a short video recorded in a home office environment.

---

## Objectives

The main objectives of this project were:

- Explore object detection capabilities using Azure AI Vision
- Analyze how the system identifies objects in different images
- Observe how detected objects change position across sequential frames from a video
- Evaluate detection results using bounding boxes and confidence scores

---

## Experiment Methodology

The experiment was conducted using **Azure Vision Studio**, which provides an interface for testing computer vision models.

The following steps were performed:

1. An Azure AI Vision resource was created in Microsoft Azure.
2. Vision Studio was opened and connected to the created Azure resource.
3. The **Object Detection** feature was selected.
4. Multiple workspace images were uploaded and analyzed.
5. Azure AI Vision generated bounding boxes and confidence scores for detected objects.
6. Detection outputs were captured as screenshots for analysis.
7. A short video of a workspace environment was recorded.
8. Three frames were extracted from the video.
9. Each frame was uploaded to Vision Studio and analyzed using the same object detection feature.

This process allowed comparison of detection results across images and video frames.

---

## Image Object Detection

Three workspace images were tested to evaluate object detection performance.

Objects detected included:

- Person
- Chair
- Monitor / Display
- Keyboard
- Table
- Plant

Azure AI Vision generated **bounding boxes around detected objects** along with **confidence scores** representing the likelihood of correct classification.

In some cases, the system classified a computer monitor as a **television**, which shows how AI models group visually similar objects.

---

## Object Tracking Using Video Frames

To demonstrate object movement, a short video was recorded in a home workspace environment.

In the video:

- A person enters the frame
- Sits at the workstation
- Waves at the camera

Three frames were extracted from the video and analyzed using Azure AI Vision.

By comparing detection results across frames, the **position of the detected person changes**, which illustrates how object detection outputs can be used to observe movement within a scene.

Although Vision Studio performs object detection on individual images, analyzing sequential frames allows a simple form of frame-based tracking.

---

## Repository Structure

```
azure-ai-vision-object-detection-tracking/

README.md

report/
        SIG788_Task5_Object_Detection_Tracking_Azure_AI_Vision.pdf

experiment-images/
        workspace_image_1.jpg
        workspace_image_2.jpg
        workspace_image_3.jpg

detection-results/
        detection_result_1.jpg
        detection_result_2.jpg
        detection_result_3.jpg

video-experiment/
        workspace_tracking_video.mp4
        frame1_original.jpg
        frame2_original.jpg
        frame3_original.jpg

frame-detection-results/
        frame1_detection.jpg
        frame2_detection.jpg
        frame3_detection.jpg
```



---

## Key Observations

- Azure AI Vision successfully detected common objects in workspace environments.
- Bounding boxes visually highlight detected objects.
- Confidence scores indicate detection reliability.
- Some objects were grouped under broader categories (e.g., monitor detected as television).
- Comparing detection results across video frames allowed observation of object movement.

---

## Conclusion

This experiment demonstrates how **Azure AI Vision** can be used to analyze images and detect objects using cloud-based computer vision services.

The results show that Azure AI Vision is capable of recognizing common objects and can support applications such as automation, surveillance, and visual scene analysis.

---

## Author

**Vijay Rodrigues**

Experiment conducted using Azure AI Vision and Vision Studio to explore computer vision capabilities.
