# Volume-and-brightness-control-for-Mac-
A Python application that lets us control system volume and screen brightness on macOS using simple hand gestures through your webcam.
Built with [Mediapipe] (https://google.github.io/mediapipe/), [OpenCV] (https://opencv.org/) and native MacOS system commands.

# Features 
- Real-time hand tracking via webcam
- **Volume control** using **right hand** gestures
- **Brightness control** using **left hand** gestures
- **Gesture toggle**: Pinch (thumb + middle finger) to enable/disable control per hand
- Smooth value transitions & system call optimization
- Visual on-screen feedback for control status

# Requirements
- MacOS (tested on MacOS Monterey and later)
- Python 3.7+
- Webcam
- [`brightness`](https://github.com/nriley/brightness) command-line tool for macOS

  Install Dependencies:
  - <code> pip install opencv-python mediapipe numpy </code>
  - install <code> brightness </brightness> using the command <code> brew install brightness </brightness>

# Usage
- Run the jupyter notebook
- Press <code> Q </code> from keyboard to quit the application

 Gesture Guide:
      | Gesture                         | Action                                       |
      | ------------------------------- | -------------------------------------------- |
      |    Thumb + Index (Right hand)   | Adjust system volume (0%–100%)               |
      |    Thumb + Index (Left hand)    | Adjust screen brightness (10%–100%)          |
      |    Thumb + Middle (Either hand) | Toggle control ON/OFF for that specific hand |

 - control is based on **distance between fingertips**
 - real-time visual feedback is shown on-screen

# To be kept in mind
- Ensure proper lighting for accurate hand detection
- Keep hands within the camera frame for constant tracking

# Future Improvements
- GUI Feedback for calibration or tracking
- Sound or visual notifications for toggling



