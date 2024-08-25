# Parking Space Detection System

This project is a computer vision-based parking space detection system developed using Python, OpenCV, and cvzone. 
The system processes video feeds to identify and display available parking spots in real-time, and includes a feature for defining and adjusting parking space positions interactively.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Usage](#usage)
- [How it works](#how-it-works)
- [Technologies Used](#technologies-used)

## Project Overview

The Parking Space Detection System is designed to monitor parking areas and detect the availability of parking spaces. 
By analyzing video footage, the system can count and highlight available parking spots, providing real-time updates on parking availability. 
Additionally, users can define or adjust the positions of parking spaces interactively through a graphical interface.

## Features

- Real-time parking space detection: Monitors video feeds and identifies free and occupied parking spaces.
- Interactive parking space positioning: Allows users to define and adjust parking space positions interactively by clicking on the image.
- Image processing: Utilizes grayscale conversion, Gaussian blur, adaptive thresholding, and other image processing techniques to enhance detection accuracy.
- Customizable display: Shows the number of available parking spaces directly on the video feed with clear visual indicators.
- Efficient data handling: Stores and retrieves parking space positions using Python's pickle module.

## Usage

- Setting Parking Space Positions </br>
  - Run the position setting script:
    ```sh
    Copy code
    python ParkingSpacePicker.py
    ```
  - Interactively define parking spaces:
    - Left-click on the image to add a new parking space.
    - Right-click on an existing parking space to remove it.
  - The positions are automatically saved to the CarParkPos file.

- Running the Detection System
  - Run the main detection script:
    ```sh
    Copy code
    python main.py
    ```
  - Watch the real-time analysis: The system will display the video feed with highlighted parking spaces,
    indicating which spots are free or occupied.

## How It Works
- Position Setting: </br> Users can interactively define or modify parking space positions on a reference image (carParkImg.png).
  The positions are stored using Python's pickle module.
- Parking Space Detection: </br> The system processes each frame of the video using a series of image processing techniques, including grayscale conversion, blurring, thresholding, and dilation.
  The processed image is analyzed to determine the occupancy of each parking space based on pixel count.
- Display and Feedback: </br> The results are displayed on the video feed, showing the number of free spaces and their locations, with dynamic visual feedback.

## Technologies Used

- Python: Programming language used for developing the system.
- OpenCV: Library used for real-time computer vision tasks
- cvzone: A utility library built on top of OpenCV to simplify common computer vision tasks.
- NumPy: Library for numerical operations, particularly useful for handling arrays and matrices.
- Pickle: Python module used for serializing and deserializing parking space positions.

## A video of the detection system

https://github.com/user-attachments/assets/69d3a511-ed9f-4e84-9a23-70fd20222429



