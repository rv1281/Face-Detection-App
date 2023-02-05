
# Face Detection App

It's a basic python app which detects user's Face, Eyes and Smile. It is coded in Python using OpenCV.

## Purpose

This app is designed to detect the face of the user by using their camera. The app will detect the face, eyes and smile of the user.
## Tech Stack

The Face detection app uses OpenCV, a computer vision and machine learning software library, and Numpy, a library for the Python programming language, for numerical computing. These technologies are utilized to detect faces, eyes, and smiles of a user through their camera.
The Face detection app uses OpenCV to capture the video from the user's webcam, and Numpy is used to manipulate the data from the webcam. OpenCV uses Haar cascades, a machine learning object detection method, to detect faces, eyes, and smiles in the webcam feed. The Haar cascade classifiers are pre-trained XML files that are loaded by OpenCV and used to identify features in the webcam feed.

When the app is running, it captures the video from the user's webcam and converts it to grayscale. The grayscale image is then passed through the Haar cascade classifier for face detection, which will identify faces in the image and draw a green rectangle around the detected faces. The same process is repeated for the eyes and smiles, using separate Haar cascade classifiers. The app will then detect eyes and smiles within the region of interest (ROI) defined by the rectangle drawn around the face. The app will then draw blue circles around the detected eyes and red rectangles around the detected smiles.

In summary, OpenCV and Numpy are used in this app to capture the video from the user's webcam, manipulate the data, and use Haar cascade classifiers to detect faces, eyes, and smiles in the webcam feed.
## Installation

- Clone the repository to your local machine.
- You need to have Python installed on your computer
- Install the required packages mentioned in the requirements.txt file by running 
```python
    pip install -r requirements.txt.
```
- Run the main file main.py 
## Running the app

- Clone the repository to your local machine
- Navigate to the project directory in your terminal
- Run the following command: ``` python main.py ```
- The app will now open a window and start the webcam, detect your - face, eyes, and smile and display the results on the window
- You can quit the app by pressing 'q' in the window.

**Note** - 
- The app uses the default camera (usually the laptop's built-in camera) for face detection. If you wish to use an external camera, you can specify the camera device index in the cv2.VideoCapture(0) line of code. For example, if you want to use the second camera, change the line to cv2.VideoCapture(1). The index of the camera starts from 0 and increments by 1 for each additional camera connected to the computer.

- The software may run a bit laggy when using a laptop's camera, and the face and eye detection boxes or circles may move slightly due to the quality of the camera. However, the performance can be improved with a higher quality camera.
## Contribution

The Face detection app is open-source and contributions are welcome. If you have an idea, found a bug, or want to improve the code, you can contribute by:

- Forking the repository
- Creating a new branch with your changes
- Submitting a pull request
Please make sure that your changes are well tested and follow the coding style used in the project.