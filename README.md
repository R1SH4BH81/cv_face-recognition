# cv_face-recognition



## Description

Welcome to the `cv_face-recognition` project! This library offers face recognition capabilities from Python and the command line. Powered by dlib's cutting-edge face recognition model, built with deep learning, it achieves an impressive accuracy of 99.38% on the Labeled Faces in the Wild benchmark.

### Features

- **Face Recognition**: The library allows you to recognize and manipulate faces efficiently.
- **State-of-the-Art Model**: It is built using dlib's state-of-the-art face recognition model, which leverages the power of deep learning for accurate results.
- **High Accuracy**: Achieving an accuracy rate of 99.38% on the Labeled Faces in the Wild benchmark, this library ensures reliable face recognition.
- **Python and Command Line**: You can utilize the face recognition capabilities either from Python or through the command line, making it versatile and user-friendly.



### Command Line Tool

This project also provides a convenient face_recognition command line tool, allowing you to perform face recognition on a folder of images directly from the command line.

## Getting Started

To use `cv_face-recognition`, follow these steps:

1. Install Dependencies: Make sure you have the required dependencies installed. The library is built using dlib's deep learning model for face recognition, so you'll need to install the necessary packages.

2. Import the Library: For Python integration, import the library in your Python script.

3. Recognize Faces: Use the library's functions to recognize and manipulate faces in images or videos.

4. Command Line Tool: If you prefer the command line interface, utilize the face_recognition command line tool to perform face recognition on a folder of images.

## Usage Examples

### Python

```python
import cv_face_recognition as cvfr

# Load image
image = cvfr.load_image("path/to/image.jpg")

# Recognize faces
face_locations = cvfr.face_locations(image)
for face_location in face_locations:
    top, right, bottom, left = face_location
    cvfr.draw_rectangle(image, top, right, bottom, left)

# Display the modified image
cvfr.show_image(image)
```

### Command Line

```
face_recognition --input_dir path/to/input_images --output_dir path/to/output_images
```

## Contribution

Contributions to this project are welcome! If you find any bugs or have ideas for improvements, feel free to create a pull request.

## Acknowledgments

This project wouldn't be possible without the outstanding work of the dlib team and the deep learning model for face recognition they've developed.

---
Created with ❤️ by the cv_face-recognition Team
