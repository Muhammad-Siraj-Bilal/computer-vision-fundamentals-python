# Computer Vision Fundamentals with Python

A practical collection of Jupyter notebooks exploring fundamental computer vision techniques using Python.

The repository progresses from basic image manipulation to more advanced detection methods, including edge detection, image thresholding, K-Means segmentation, HOG with SVM for people detection and MTCNN for face detection.

## Project Overview

Computer vision enables computers to extract useful information from images and videos.

This repository demonstrates several important computer vision concepts through practical notebook-based exercises. Each notebook focuses on a specific technique and includes code, visual outputs and examples to explain how the method works.

## Topics Covered

* Reading and displaying digital images
* Understanding image dimensions and colour channels
* Image resizing, cropping and transformations
* Image filtering and smoothing
* Grayscale and colour-space conversion
* Edge detection
* Binary and adaptive thresholding
* Image segmentation using K-Means clustering
* Histogram of Oriented Gradients
* Support Vector Machine-based people detection
* Face detection using MTCNN

## Repository Structure

```text
computer-vision-fundamentals-python/
├── 01_image_operations_basics.ipynb
├── 02_image_transformations_and_filters.ipynb
├── 03_edge_detection.ipynb
├── 04_image_thresholding.ipynb
├── 05_kmeans_image_segmentation.ipynb
├── 06_hog_svm_people_detection.ipynb
├── 07_mtcnn_face_detection.ipynb
├── assets/
├── requirements.txt
├── .gitignore
└── README.md
```

## Notebook Guide

| Notebook                                     | Description                                                                                        |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `01_image_operations_basics.ipynb`           | Introduces basic image loading, display, dimensions, pixels and colour channels.                   |
| `02_image_transformations_and_filters.ipynb` | Demonstrates image resizing, cropping, transformations, smoothing and filtering operations.        |
| `03_edge_detection.ipynb`                    | Explores methods for identifying object boundaries and important structural information in images. |
| `04_image_thresholding.ipynb`                | Applies thresholding techniques to separate foreground objects from image backgrounds.             |
| `05_kmeans_image_segmentation.ipynb`         | Uses K-Means clustering to group similar pixels and segment images into colour-based regions.      |
| `06_hog_svm_people_detection.ipynb`          | Demonstrates people detection using Histogram of Oriented Gradients and Support Vector Machines.   |
| `07_mtcnn_face_detection.ipynb`              | Uses Multi-task Cascaded Convolutional Networks to detect faces and facial landmarks.              |

## Technologies Used

* Python
* Jupyter Notebook
* OpenCV
* NumPy
* Matplotlib
* Scikit-image
* Scikit-learn
* TensorFlow
* MTCNN
* Pillow

## Installation

Clone the repository:

```bash
git clone https://github.com/Muhammad-Siraj-Bilal/computer-vision-fundamentals-python.git
cd computer-vision-fundamentals-python
```

Create a Python virtual environment:

```bash
python -m venv venv
```

Activate the environment on Windows:

```bash
venv\Scripts\activate
```

Activate it on macOS or Linux:

```bash
source venv/bin/activate
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Alternatively, install the main packages manually:

```bash
pip install jupyter opencv-python numpy matplotlib scikit-image scikit-learn pillow mtcnn tensorflow
```

## Running the Notebooks

Start Jupyter Notebook:

```bash
jupyter notebook
```

A browser window will open showing the repository files.

Open any notebook and run the cells in order using:

```text
Shift + Enter
```

The notebooks are numbered to provide a recommended learning sequence, beginning with basic image operations and progressing towards object and face detection.

## Suggested `requirements.txt`

```text
jupyter
numpy
matplotlib
opencv-python
scikit-image
scikit-learn
Pillow
mtcnn
tensorflow
```

Package versions may be added later to improve reproducibility.

## Image Assets

Some notebooks may require local images for demonstrations.

Create an `assets` directory:

```text
assets/
├── sample_image.jpg
├── sample_portrait.jpg
├── people.jpg
└── group_photo.jpg
```

Update notebook image paths to use the assets directory:

```python
image = cv2.imread("assets/sample_image.jpg")
```

Only upload images that you created or have permission to redistribute.

## Key Concepts

### Image Operations

Digital images are represented as arrays of pixel values. The introductory notebooks demonstrate how to read, inspect, modify and display these arrays using Python and OpenCV.

### Image Transformations and Filtering

Image transformations change an image's dimensions, position or orientation. Filters can reduce noise, smooth an image or highlight important visual features.

### Edge Detection

Edge detection identifies areas where image intensity changes significantly. These changes often represent boundaries between objects or regions.

### Image Thresholding

Thresholding converts an image into separated regions based on pixel-intensity values. It is commonly used to isolate foreground objects from backgrounds.

### K-Means Image Segmentation

K-Means clustering groups pixels with similar colour or intensity values. This creates a simplified image containing a selected number of colour regions.

### HOG and SVM

Histogram of Oriented Gradients describes the direction and distribution of edges within an image. These features can be used with a Support Vector Machine to identify people or other objects.

### MTCNN Face Detection

MTCNN is a deep-learning face-detection approach that uses a sequence of neural networks to locate faces and identify important facial landmarks.

## Learning Outcomes

Through these notebooks, users can learn how to:

* Load and manipulate images using Python
* Apply common preprocessing operations
* Extract edges and structural features
* Segment images into meaningful regions
* Understand traditional feature-based object detection
* Apply pretrained deep-learning face detectors
* Display and interpret computer vision outputs
* Use Jupyter Notebook for practical image analysis

## Current Limitations

* Some notebooks depend on local image files
* Results may vary depending on image quality
* The notebooks are intended primarily for learning and experimentation
* Detection methods have not been evaluated on a formal benchmark dataset
* Some examples may require adjustments for newer library versions
* The repository does not currently provide a unified application interface

## Future Improvements

* Add an organised `assets` folder
* Add explanatory Markdown cells to each notebook
* Include sample input and output images
* Add webcam-based real-time detection
* Compare multiple edge-detection algorithms
* Add contour and shape detection
* Add object detection using YOLO
* Add image classification using convolutional neural networks
* Create a Streamlit computer vision demonstration application
* Add automated environment and dependency testing

## Educational Purpose

This repository was developed for educational and portfolio purposes to demonstrate fundamental computer vision concepts using practical Python examples.

The notebooks are designed to support learners who are beginning their journey in image processing, machine learning and computer vision.

## Author

**Muhammad Siraj Bilal**

## Licence

This repository is intended for educational and research use.

Add an open-source licence such as the MIT Licence if you plan to allow others to reuse, modify or distribute the code.
