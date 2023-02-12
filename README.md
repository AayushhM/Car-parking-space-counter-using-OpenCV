
# Car Park Occupancy Detection System

This project is designed to detect the occupancy status of a car park in real-time. The system uses a video of the car park and detects the presence of a car in each parking slot by analyzing the video frames.

Step 1: Creating the Parking Slot Locations
In this step, we manually select the parking slot locations in an image of the car park. The selected parking slot locations are stored in a file named CarParkPos using the Python pickle library.

Step 2: Monitoring the Car Park Occupancy
In this step, we read the video of the car park and for each frame, we check the occupancy status of each parking slot. We use image processing techniques to detect the presence of a car in the parking slot. 
The techniques used are:
Converting the frame from BGR to grayscale,
Applying Gaussian Blur to remove noise,
Adaptive thresholding to separate the background and foreground,
Median Blur to remove salt and pepper noise,
Dilation to expand the detected object, 
Finally, we draw a rectangle around the parking slot and color it green if it is empty and red if it is occupied. The number of free parking slots and the total number of parking slots are displayed on the output video.

Conclusion:
The Car Park Occupancy Detection System can accurately detect the occupancy status of a car park in real-time. The system is robust and can handle different lighting conditions and movements in the video.


## Screenshots

![App Screenshot](https://user-images.githubusercontent.com/13918412/218334986-99952f64-d1da-4789-aabe-b83241336618.png)

