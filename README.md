# Facial Landmark Detection

- This project demonstrates facial landmark detection using the cv2, and dlib library in Python. 
- It utilizes a pre-trained model to detect facial landmarks on a live video stream from a computer's camera.
- The pre-trained model is extracted from [here](https://github.com/italojs/facial-landmarks-recognition/blob/master/shape_predictor_68_face_landmarks.dat).
- Make sure to insert the raw file in the root folder (or any folder as long as the path is mentioned in the following code).
  ```python
  predictor = dlib.shape_predictor("shape_predictor_68_face_landmarks.dat")
  ```
## Requirements

Make sure you have the following libraries installed:

- opencv
- dlib

You can install them using the command:
- For OpenCV (for usage of cv2)
```bash
pip install opencv
```
- For dlib make sure to have their dependencies installed as well
  - On Linux and MacOS based system
  ```bash
  sudo apt-get install cmake
  sudo apt-get install build-essential
  ```
  - On Windows (for python 3.7+) install dlib from [here](https://github.com/sachadee/Dlib#dlib-compiled-wheels-for-python-37-38-39-for-windows-10-x64).
    - Clone the repo
    - cd to Dlib
    - Install based on Python version.
    - Below is an example script for Python version 3.7.x
    ```bash
    python -m pip install dlib-19.22.99-cp37-cp37m-win_amd64.whl 
    ```
## Usage

1. Clone the repository:

```bash
git clone https://github.com/prashantgarbuja/facial-landmark-detection.git
```

2. Navigate to the project directory:

```bash
cd facial-landmark-detection
```

3. Run the Python script (After installing all the dependencies):

```bash
python facial_landmark_detection.py
```

4. The script will open your computer's camera feed, and you'll see facial landmarks overlaid on detected faces.
   <p align="center">
    <img src="https://github.com/prashantgarbuja/facial-landmark-detection/blob/main/face_landmark.png" />
  </p>
 
 ## Additional Notes

- The `shape_predictor_68_face_landmarks.dat` file contains the pre-trained model for facial landmark detection. Ensure it is in the same directory as your Python script.

- Press `q` to exit the video stream.

- Feel free to customize the code for your specific use case or integrate it into other projects.

## Acknowledgments

- [dlib library](http://dlib.net/): A toolkit for machine learning and computer vision tasks.

- [OpenCV library](https://opencv.org/): An open-source computer vision and machine learning software library.
