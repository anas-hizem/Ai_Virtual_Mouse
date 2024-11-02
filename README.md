# Virtual Mouse Control with Hand Tracking

## Overview
This project implements a virtual mouse control system that allows users to control the mouse cursor on their computer screen using hand gestures. It utilizes OpenCV for image processing, Mediapipe for hand tracking, and Autopy for mouse control. The project enables intuitive interaction with computer interfaces, making it useful in various scenarios, such as presentations, touchless interfaces, and accessibility applications.

## Features
- Hand tracking using Mediapipe.
- Mouse movement control with index finger gestures.
- Click functionality using finger distance detection.
- Real-time performance metrics (FPS display).
- Smooth cursor movement for better user experience.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Prerequisites
Before running the project, ensure you have the following installed:
- Python 3.6 or higher
- pip (Python package manager)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/virtual-mouse-control.git
   cd virtual-mouse-control
   ```
2.Install the required packages:
```bash
pip install opencv-python numpy mediapipe autopy
```


## Usage :
1. Connect a camera to your computer (internal or external)
2. Run the main script:

```bash
python AiVirtualMouse.py
```
3. Position your hand in front of the camera to control the mouse cursor.
4. Raise your index finger to move the cursor and click by bringing the index and middle fingers close together.

## Project Structure:
```bash
virtual-mouse-control/
├── AiVirtualMouse.py          # Main script for virtual mouse control
├── HandTrackingModule.py      # Module for hand detection and gesture recognition
├── AiVirtualMouseProject.py   # (Optional) Duplicate of the main script for testing
├── README.md                  # Project documentation
```


## How It Works :

1. **Camera Setup**: The program initializes the camera with specified dimensions.
2. **Hand Detection**: Using the handDetector class from the HandTrackingModule, the program detects hand landmarks in real-time.
3. **Mouse Movement**:
- If the index finger is raised, the cursor moves based on the finger's position.
- If the index and middle fingers are close enough, a mouse click is registered.
4. **Performance Monitoring**: The program calculates and displays the frames per second (FPS) of the video feed.


## Gesture Logic :
- **Mouse Movement**: The index finger's position is tracked to move the cursor.
- **Mouse Click**: The distance between the index and middle fingers determines if a click is made.

## Contributing :
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes. You can also report issues or suggest features by opening an issue on GitHub.

## Acknowledgments
- **OpenCV** for image processing capabilities.
- **Mediapipe** for hand tracking.
- **Autopy** for mouse control.










