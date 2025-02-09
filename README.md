
# Face Recognition Image Capture

This project captures images from a webcam and saves them in a specified directory, to be used later for face recognition tasks. The script captures up to 100 images, detects faces, and stores them in an organized manner with the person's name and ID.

## Requirements

- Python 3.x
- OpenCV (cv2)
- Haarcascade for face detection (`haarcascade_frontalface_default.xml`)

### Installation

1. **Install Python 3**: Make sure Python 3.x is installed on your system.

2. **Install OpenCV**:
   ```bash
   pip install opencv-python
   ```

3. **Download Haarcascade File**:
   Download the `haarcascade_frontalface_default.xml` file from OpenCV's official repository [here](https://github.com/opencv/opencv/tree/master/data/haarcascades).

4. **Create the project directory**:
   Create a folder where you will store the captured images. The script will create a subfolder based on the provided name and ID to save images.

## Usage

1. **Run the script**:
   - The script will ask you to enter your name and ID.
   - It will then start capturing images from your webcam. It will save each detected face in the specified folder.

2. **Start capturing images**:
   - Once the webcam is activated, it will start capturing up to 100 images, which will be saved under the folder `images/[nameid]/'.

   ```python
   python capture_faces.py
   ```

3. **Images will be saved in the following format**:
   - `images/[nameid]/1.jpg`
   - `images/[nameid]/2.jpg`
   - ...
   - `images/[nameid]/100.jpg`

## How It Works

1. The script starts by capturing live video from the webcam.
2. It detects faces in the frame using OpenCV's `CascadeClassifier`.
3. For each detected face, it saves the image in the designated folder.
4. Once 100 images are captured, it stops.

## Troubleshooting

- **Camera not detected**: Make sure your camera is working and properly connected.
- **No faces detected**: Ensure that your face is properly visible in the webcam frame.


