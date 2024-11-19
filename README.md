# 🅿️ Parking Slot Detection System Using MATLAB

This MATLAB-based project detects and counts available parking spaces in a parking lot using **image processing techniques**. It showcases the potential for automated parking management systems and can be extended for real-time monitoring using live camera feeds. 🚗🅿️

---

## 📜 **Introduction**
The **Parking Slot Detection System** is a MATLAB application designed to analyze parking lot images, distinguishing between **vacant** and **occupied slots**. By leveraging MATLAB's powerful image processing tools, the system demonstrates how technology can simplify parking management in **urban areas**, **shopping malls**, **airports**, and more.

---

## 🎯 **Project Objective**
The main goal is to build a functional system that:
- Detects available parking spaces from an uploaded image.
- Uses image processing to identify and count vehicles.
- Displays the results in an easy-to-understand format with MATLAB's **Graphical User Interface (GUI)**.

![Parking Lot Image](https://github.com/user-attachments/assets/832becd9-c4dd-47d9-a83b-3549970773b8)

---

## ⚙️ **Project Features**

### **1. User-Friendly MATLAB GUI**
- Intuitive interface designed with MATLAB's GUIDE tool.
- Allows users to upload parking lot images, view results, and monitor vacant slots in real time.

### **2. Image Processing Techniques**
- **Grayscale Conversion**: Simplifies image processing by converting the input image to grayscale.
- **Thresholding**: Differentiates between the parking lot background and vehicles.
- **Binary Image Conversion**: Converts the grayscale image into a black-and-white binary format for easier analysis.
- **Object Detection**: Detects and labels connected components (vehicles) using MATLAB's `bwlabel` function.

### **3. Parking Slot Counter**
- Dynamically calculates and displays the number of vacant parking slots based on the detected vehicles and total slots.

---

## 🔍 **How the System Works**

1. **Image Upload**: Users upload an image of the parking lot via the GUI.
2. **Image Preprocessing**: 
   - Convert the image to grayscale.
   - Apply thresholding and binary conversion.
3. **Vacant Slot Detection**:
   - Detect vehicles using object detection techniques.
   - Calculate available slots by subtracting detected vehicles from total slots.
4. **Results Display**: The processed image and the number of vacant slots are displayed in the GUI.

![Workflow Image 1](https://github.com/user-attachments/assets/1f6affb1-7fd7-4cb5-8966-7c36185176b4)
![Workflow Image 2](https://github.com/user-attachments/assets/7ad4e530-1f92-416c-b4e1-513d70c51be6)
![Workflow Image 3](https://github.com/user-attachments/assets/37bf53c6-0c69-4d79-9d8c-519e9ae86591)

---

## 📂 **File Descriptions**

### **1. untitled1.m**
- The main MATLAB script powering the system.
- Key functions:
  - **`untitled1_OpeningFcn`**: Initializes the GUI and system variables.
  - **`pushbutton1_Callback`**: Handles image upload and displays it on the GUI.
  - **`pushbutton2_Callback`**: Executes the parking slot detection algorithm and updates the results.

### **2. untitled1.fig**
- The figure file defining the GUI layout.
- Includes components like:
  - **Buttons** for uploading images and running the detection algorithm.
  - **Axes** for displaying images and results.
  - **Text fields** for showing the number of vacant slots.

![GUI Design](https://github.com/user-attachments/assets/f5c27290-64a3-4746-b35d-631f1d604983)
![GUI in Action](https://github.com/user-attachments/assets/dfd0262e-ca84-49a5-a8c0-2028a1fd0e9a)

---

## 🛠️ **Use Cases**
1. **Parking Management**: Monitor real-time parking lot occupancy.
2. **Traffic Monitoring**: Extend the project for vehicle detection in traffic scenarios.
3. **Smart Cities**: Integrate with smart city systems to optimize parking availability and reduce congestion.

---

## 🚀 **Future Improvements**
1. **Real-Time Monitoring**:
   - Integrate live camera feeds for continuous parking lot monitoring.
2. **Machine Learning**:
   - Use advanced models to improve detection accuracy in complex environments.
3. **Multi-Lot Management**:
   - Track multiple parking lots simultaneously from a centralized dashboard.

---

## 📜 **How to Use**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/touhidulislam1999/Parking-Slot-Detection-System-Using-MATLAB.git
