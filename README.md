# **Project Title: Shape Detection and Symmetry Creation**

## **Table of Contents**
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Project Structure](#project-structure)
5. [Examples](#examples)

## **Introduction**
This project is focused on detecting various 2D shapes in raster images, drawing symmetry lines, and completing incomplete curves using image processing techniques. The primary goal is to automate the identification and manipulation of shapes within an image, creating a complete and symmetrical representation.

## **Features**
- **Shape Detection**: Automatically detects and labels different shapes (triangles, rectangles, circles, etc.) in a given image.
- **Symmetry Line Drawing**: Draws horizontal and vertical symmetry lines through the center of an image.
- **Symmetrical Image Creation**: Generates a full symmetrical image by mirroring one half of an image.
- **Curve Completion**: Completes an incomplete curve using spline fitting techniques to reconstruct the missing parts.

## **Installation**
To run this project, you'll need to install Python along with the following libraries using the command in CLI:
```bash
pip install opencv-python matplotlib numpy scipy
```

## **Project Structure**

This project consists of the following main scripts:

- `shape_detection.py`: Contains the code for detecting and labeling 2D shapes within an image. It utilizes the OpenCV library to read images, convert them to grayscale, apply thresholding, and detect contours to identify and classify shapes like triangles, rectangles, circles, etc.

- `symmetry_lines.py`: This script is responsible for drawing vertical and horizontal symmetry lines on an image. It calculates the center points of the image and draws lines through these centers, helping to visualize the symmetry.

- `symmetrical_image.py`: Generates a complete symmetrical image by mirroring one half of a given image. The script first cuts the image in half and then creates a mirrored version to complete the other side, resulting in a fully symmetrical image.

- `curve_completion.py`: Implements a method for completing incomplete curves using spline fitting. This script detects the contour of the incomplete curve, sorts and fits a spline to the detected points, and then reconstructs the missing parts of the curve.

## **Examples**

Here are some examples showcasing the capabilities of this project:

### **Shape Detection**

In this example, the script detects various shapes such as triangles, rectangles, and circles in an image. It labels each shape accordingly and displays the result.

**Sample Output:**
```plaintext
Shape detected: Triangle
Shape detected: Rectangle
Shape detected: Circle
