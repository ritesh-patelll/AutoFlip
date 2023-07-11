# AutoFlip

This tool uses AI-based object detection to identify the main action parts in each frame of a video and smartly crops it to ensure no loss of important elements. For face and pose detection it uses MediaPipe, a flexible framework that contains machine learning solutions for live and streaming media.

<p align="center">
  <img src="/demo/BeforeAutoFlip1.gif" alt="GIF" width="40%">
  ----------------->
  <img src="/demo/AfterAutoFlip1.gif" alt="GIF" height="230px">
</p>

<p align="center">
  <img src="/demo/BeforeAutoFlip2.gif" alt="GIF" width="40%">
  ----------------->
  <img src="/demo/AfterAutoFlip2.gif" alt="GIF" height="230px">
</p>

---

## Features:
1. Google-Colaboratory compatible.
2. Works on any video, regardless of its initial aspect ratio.
3. AI-based automatic cropping.
4. "Face detection" and "Pose landmarks detection" using MediaPipe.
5. Audio preservation: Extracts the audio from the original video and attaches it to the output video.
6. Dynamic video splitting: Automatically chunks the video into segments based on changes in the background.

## Dependencies:
1. `cv2`
2. `os`
3. `numpy`
4. `mediapipe`
5. `moviepy`

## Usage:

1. Clone the repository

```sh
git clone https://github.com/user/autoflip.git
```

2. Install dependencies

```sh
pip install opencv-python
```

```sh
pip install numpy
```

```sh
pip install mediapipe
```

```sh
pip install moviepy
```

3. Run Detector.py

## Need improvement:

1. *Rotation of frames:* If the video includes frames that need to be rotated to fit the correct orientation, consider adding an orientation detection model. For instance, you could train a CNN on a dataset of images that are manually marked for orientation.

2. *Auto-Scaling:* This feature configures the video scaling automatically based on the detected face or object in the frame to optimize the visible area of interest.

3. *Frame Interpolation:* This is a technique where you generate intermediate frames between the two existing ones. This could make your resulting video smoother.

4. *Noise Reduction:* Implement a noise reduction technique to improve the quality of video.

5. *Optimization:* Consider optimizing your code further to increase the speed of the processing time. You can profile your code to find bottlenecks and then address those.

Remember, the introduction of these features might add complexity to the code and may increase processing time. So make sure you thoroughly test any new additions.

## Contributing:
Pull requests are always welcome. Feel free to `fork` this repo.

## License:

This project is licensed under the terms of the MIT license.

Note: This script does not handle graphical user input yet. It should be run from the command line using the arguments specified in the script.
