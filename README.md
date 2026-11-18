
# Real-Time Colour Detection Using Python and OpenCV

A computer vision project that detects and identifies different colours in real time using a webcam. Developed using Python, OpenCV and NumPy, this application processes live video frames and highlights detected colour regions with bounding boxes and labels.

---

## About the Project

Colour detection is an important application of image processing and computer vision. It allows a computer system to identify specific colours from images or live video streams.

The main aim of this project is to develop a simple real-time colour detection system that uses a webcam to identify selected colours from the surrounding environment.

The application captures live video, converts each frame into HSV (Hue, Saturation and Value) colour space, and identifies colours using predefined threshold ranges. Once a colour is detected, the program highlights the corresponding region with a bounding box and displays its name on the screen.

The project was developed as part of the Minor Image Processing coursework.

## Project Objectives

- To understand the basic concepts of image processing and computer vision.
- To implement real-time colour detection using Python and OpenCV.
- To understand the HSV colour model and its role in colour identification.
- To capture and process live video using a webcam.
- To identify selected colours and highlight their regions.
- To improve detection quality through basic noise reduction techniques.

## Technologies Used

| Technology | Description |
|---|---|
| Python | Used to develop the application. |
| OpenCV | Used for image processing and computer vision operations. |
| NumPy | Used for numerical operations and array manipulation. |
| HSV Colour Space | Used to identify colours based on their HSV ranges. |
| Visual Studio Code | Used as the development environment. |

## Features

The application includes the following features:

- Real-time video capture through a webcam.
- Detection of five predefined colours: Red, Orange, Green, Blue and Yellow.
- Colour identification using HSV thresholding.
- Noise reduction using morphological operations.
- Contour detection to identify colour regions.
- Bounding boxes and colour labels around detected regions.
- Minimum area filtering to ignore smaller unwanted regions.

## How It Works

The system follows a series of image processing steps to identify colours from a live webcam feed.

**1. Webcam Capture**

The application accesses the system webcam and continuously captures video frames.

**2. Conversion to HSV Colour Space**

Each captured frame is converted from BGR colour space to HSV. HSV makes it easier to identify colours using separate hue, saturation and brightness values.

**3. Colour Detection**

Predefined HSV ranges are used to create masks for the selected colours. These masks help isolate pixels that fall within the specified colour ranges.

**4. Noise Reduction**

Morphological operations such as opening and closing are applied to reduce unwanted noise and fill small gaps in the detected regions.

**5. Contour Detection**

The system identifies the boundaries of the detected colour regions using OpenCV contour detection.

**6. Area Filtering**

Small detected regions are filtered out using a minimum contour area threshold to reduce unnecessary detections.

**7. Display of Results**

Finally, bounding boxes and corresponding colour labels are drawn around the detected regions and displayed on the live webcam feed.

## Project Structure

```text
Color-Detection-Using-OpenCV/
│
├── main.py
├── requirements.txt
├── README.md
├── .gitignore
└── .venv/ 
```

The `.venv` folder is created locally when setting up the Python environment and is not included in the GitHub repository.

## Installation and Setup

Follow these steps to run the project on your system.

**Step 1: Clone the repository**

```bash
git clone https://github.com/TED-GUSINGE/Color-Detection-Using-OpenCV.git
```

**Step 2: Open the project directory**

```bash
cd Color-Detection-Using-OpenCV
```

**Step 3: Create a virtual environment**

```bash
python3 -m venv .venv
```

**Step 4: Activate the virtual environment**

For macOS and Linux:

```bash
source .venv/bin/activate
```

For Windows:

```bash
.venv\Scripts\activate
```

**Step 5: Install the required libraries**

```bash
python -m pip install -r requirements.txt
```

**Step 6: Run the application**

```bash
python main.py
```

Make sure your webcam is connected and camera permissions are enabled. Press the `Q` key to close the application.

## Applications

Colour detection can be useful in several areas, including:

- Basic object identification systems.
- Computer vision and image processing applications.
- Colour-based sorting systems.
- Educational demonstrations of image processing.
- Robotics and automation experiments.

## Limitations

Although the application performs real-time colour detection, there are certain limitations:

- Detection accuracy can vary depending on lighting conditions.
- Camera quality and exposure may affect colour identification.
- Similar colour shades can sometimes be classified incorrectly.
- Red and orange may have overlapping HSV ranges, which can lead to occasional misclassification.
- The system uses predefined colour thresholds rather than machine learning-based object recognition.

## Future Improvements

The project can be further developed by introducing:

- Interactive HSV calibration for more accurate colour detection.
- Improved handling of similar colour shades.
- Support for additional colour categories.
- Object tracking capabilities.
- A more interactive graphical user interface.

## Conclusion

This project demonstrates how basic image processing techniques can be used to build a real-time colour detection application.

By combining Python, OpenCV and NumPy, the system is able to capture live video, identify selected colours and highlight their corresponding regions.

Working on this project provided practical experience with webcam integration, HSV colour space, image segmentation, morphological operations and contour detection.

---

## Author

**Tejas Gusinge**

B.Tech – Computer Science and Engineering

Ajeenkya D. Y. Patil University, Pune

**Project:** Minor – Image Processing

---

*Developed as an academic mini-project.*
