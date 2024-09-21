# Parking-Slot-Detection-System-Using-MATLAB
The project is a MATLAB-based application that uses image processing techniques to detect and count available parking spaces in a parking lot. It displays vacant spots and demonstrates the potential of automated parking management systems, which can work with live camera feeds for real-time monitoring.

# Introduction:
The Parking Slot Detection System is a MATLAB-based project designed to detect and count available parking spaces in an image of a parking lot. The project leverages image processing techniques to analyze parking lot images, distinguishing between occupied and vacant slots. This system is ideal for creating a real-time parking management tool that could be further extended to integrate with live camera feeds for smart parking solutions in urban areas, shopping malls, airports, etc.

# Project Objective:
The primary objective of this project is to build a functional model for detecting available parking slots in an image and to demonstrate the potential for parking management automation. Using MATLAB's built-in functions, the system allows for easy image upload, processing, and results visualization, giving the user a clear and informative output about the parking lot occupancy.

# Project Features:
**User-Friendly MATLAB GUI:****
- Item 1 The system has a simple and intuitive Graphical User Interface (GUI) designed using MATLAB's GUIDE tool. The interface enables users to interact with the application by uploading images, viewing processed outputs, and seeing the number of detected vacant slots in real-time.
Image Processing Techniques:
Grayscale Conversion: Once the user uploads an image of a parking lot, it is first converted into a grayscale image to simplify further processing.
Thresholding: A global threshold is applied to differentiate the background from objects (i.e., vehicles) in the image.
Binary Image Conversion: The grayscale image is converted into a binary image (black and white) where parking spots are segmented for further analysis.
Object Detection & Labeling: Using MATLAB’s bwlabel function, the system detects and labels each object in the binary image to count the number of vehicles and thus calculate the available parking spaces.
Parking Slot Counter:
The system identifies vacant spots by calculating the total number of parking spaces in the image and subtracting the number of detected vehicles. This information is dynamically updated in the GUI, providing real-time feedback to the user.
How the System Works:
Step 1: Image Upload: The user selects an image of the parking lot using the GUI’s file upload function.
Step 2: Image Preprocessing: The image is read into the program and converted to a grayscale format. This makes it easier to apply thresholding and identify vehicles.
Step 3: Thresholding & Binary Conversion: A thresholding technique is applied to the grayscale image to convert it into a binary (black and white) image, where the parking lot and vehicles can be separated for detection.
Step 4: Vacant Slot Detection: The binary image is processed using object detection techniques. The bwlabel function labels connected components in the image, detecting cars and calculating the number of available parking slots.
Step 5: Results Display: The processed image, showing detected vehicles, is displayed in the GUI. The count of available parking slots is dynamically updated and displayed as well.
File Descriptions:
untitled1.m:
This is the main MATLAB script that powers the parking detection system. It contains the code for the GUI and the core functions responsible for image loading, preprocessing, and slot detection.
Key functions include:
untitled1_OpeningFcn: Initializes the GUI and sets up necessary variables and structures.
pushbutton1_Callback: Handles the image upload functionality and displays the uploaded image on the GUI.
pushbutton2_Callback: Executes the parking slot detection logic, counting the number of vacant slots and displaying the result in the GUI.
untitled1.fig:
This is the associated figure file for the GUI layout. It defines the layout of the buttons, axes for image display, and text fields where the parking results are shown.
Use Cases:
Parking Management System: This project could be adapted to monitor real-time parking lot occupancy. With modifications, it could connect to live video feeds to continuously monitor and update available parking slots.
Traffic Monitoring: The project can be extended to detect other forms of vehicles or traffic patterns in real time.
Smart City Solutions: This system could be part of a larger smart city initiative, helping optimize parking spaces in urban environments and reducing congestion caused by drivers searching for parking.
Future Improvements:
Real-Time Integration: Extend the project by integrating with live camera feeds, enabling real-time detection and monitoring of parking spaces.
Machine Learning: Implement machine learning models to enhance the accuracy of vehicle detection and slot recognition, especially in more complex parking lot images.
Multi-Lot Monitoring: Allow the system to handle multiple parking lots at once, tracking the available spots in different locations from a central dashboard.
