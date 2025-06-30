# Face Detection and Analysis Project

## Overview

This project focuses on face detection and analysis in digital images using deep learning techniques, specifically leveraging a Deep Neural Network (DNN) model. 
The primary goal is to detect faces in images, extract facial features such as skin and eye color, and perform clustering based on these features. The project utilizes OpenCV for image processing and a pre-trained DNN model (res10_300x300_ssd_iter_1400000.caffemodel with deploy.prototxt.txt) for face detection. 
The extracted features are processed in the YCrCb color space for skin detection and RGB for eye color classification.v

## Features


- Face Detection: Uses a pre-trained DNN model to identify faces in digital images, handling various angles and orientations effectively.



- Skin Color Extraction: Converts images to YCrCb color space, applies a skin mask, and calculates the average RGB color of the detected skin region within a bounding box.



- Eye Color Detection: Extracts the eye region using bounding box coordinates, converts it to RGB format, and computes the average color, categorizing it into predefined classes (brown, blue, green, hazel, gray, amber).



- Clustering Analysis: Performs clustering on extracted features to group similar images, with results visualized through heatmaps and cluster statistics.



- Bounding Box Adjustment: Utilizes the mean of other bounding boxes to refine detection in cases where direct detection may fail due to image angles.



- Eye Position Analysis: Ensures consistent eye positioning across images using a coefficient-based approach for accurate feature extraction.



- Comprehensive Image Processing: Handles multiple test and train images, generating heatmaps of feature means by cluster for analysis.
