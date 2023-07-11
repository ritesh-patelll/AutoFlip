# AutoFlip

This tool uses AI-based object detection to identify the main action parts in each frame of a video and smartly crops it to ensure no loss of important elements. For face and pose detection it uses MediaPipe, a flexible framework that contains machine learning solutions for live and streaming media.

<p align="center">
  <img src="/demo/BeforeAutoFlip1.gif" alt="GIF" width="40%">
  ----------------->
  <img src="/demo/AfterAutoFlip1.gif" alt="GIF">
</p>

<p align="center">
  <img src="/demo/BeforeAutoFlip2.gif" alt="GIF" width="40%">
  ----------------->
  <img src="/demo/AfterAutoFlip2.gif" alt="GIF" width="40%">
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
pip install -r requirements.txt
```

3. Run Detector.py

## Screenshots:
Visual Demonstrations of the before-and-after are recommended.

## Contributing:
Pull requests are always welcome. Feel free to `fork` this repo.

## License:

This project is licensed under the terms of the MIT license.

Note: This script does not handle graphical user input yet. It should be run from the command line using the arguments specified in the script.
