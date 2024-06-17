# Face Mask Detection Project

## Overview

This project is a real-time face mask detection system that uses deep learning models to accurately detect whether individuals in images and videos are wearing masks. The system leverages Convolutional Neural Networks (CNNs) to classify faces into mask and no-mask categories. The primary goal of this project is to develop a robust and efficient system for real-time mask detection to aid in public health measures.

## Technologies Used

- **OpenCV**: For image processing and face detection.
- **Keras**: For building and training deep learning models.
- **TensorFlow**: As the backend for Keras to leverage its powerful deep learning capabilities.
- **Imutils**: For easy image processing and video stream handling.

## Installation

To get started with this project, follow the instructions below to set up your environment.

### Prerequisites

Ensure you have the following installed:

- Python (3.6+)
- Anaconda (Recommended for managing packages and environments)

### Clone the Repository

```bash
git clone https://github.com/yourusername/FaceMaskDetection.git
```

## Create a Virtual Environment

```bash
conda create -n mask-detection python=3.8
conda activate mask-detection
```

## Install Dependencies
```bash
pip install -r requirements.txt
```

## Download Face Detector Model

Ensure you have the face detector model files in the `face_detector` directory:
`deploy.prototxt` & `res10_300x300_ssd_iter_140000.caffemodel`

You can download them from this <a href="https://github.com/opencv/opencv/tree/master/samples/dnn/face_detector">link.</a>

## Download Pre-trained Mask Detector Model

Ensure you have the trained face mask detector model:
`trained_model.h5`

You can download it from this <a href="https://github.com/amirhalijani/FaceMaskDetection/blob/main/trained_model.h5">link.</a>

## Usage

To test the project, run the following command (replace the path to Python executable with the location where Anaconda is installed on your system):
```bash
C:\ProgramData\anaconda3\python.exe mask_detector_video.py
```

### Arguments
- **--face**: Path to the face detector directory.
- **--model**: Path to the trained face mask detector model.
- **--confidence**: Minimum probability to filter weak detections (default: 0.5).

#### Example Command:
```bash
C:\ProgramData\anaconda3\python.exe mask_detector_video.py --face face_detector --model trained_model.h5 --confidence 0.5
```

## How to Run the Code

Ensure all dependencies are installed and the necessary model files are downloaded.

Activate your virtual environment.

Run the command provided above to start the video stream and detect face masks in real-time.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Acknowledgements

OpenCV for providing a robust library for computer vision tasks.

Keras and TensorFlow teams for their powerful deep learning frameworks.

The open-source community for their contributions and support.
