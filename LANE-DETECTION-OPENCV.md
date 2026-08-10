# LANE-DETECTION-OPENCV

Lane detection for autonomous vehicles using OpenCV

## Summary
This project implements a lane detection pipeline using classical computer vision techniques with OpenCV. The goal is to detect lane boundaries in road images or video feeds and overlay the detected lanes for visualization.

## Motivation
Lane detection is a core component of driver assistance systems and autonomous driving stacks. This project demonstrates a real-time-capable, lightweight method that works well on clear road scenes.

## Key Features
- Camera input: process single images, video files, or webcam stream
- Preprocessing: color selection, grayscale conversion, Gaussian blur
- Edge detection: Canny edge detector
- ROI masking: focus on region where lanes are expected
- Line detection: Hough transform to detect lane lines
- Post-processing: averaging and extrapolating lane lines, smoothing across frames

## Technologies
- Python 3
- OpenCV
- NumPy
- Matplotlib (for visualizations)

## Installation
1. Clone the repository
   ```bash
   git clone https://github.com/chirravamshi/academic-projects.git
   cd academic-projects/LANE-DETECTION-OPENCV
   ```
2. Create virtual environment and install dependencies
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

## Usage
- Process an image:
  ```bash
  python detect.py --input images/test1.jpg --output out/test1_out.jpg
  ```
- Process a video:
  ```bash
  python detect.py --input videos/road.mp4 --output out/road_out.mp4
  ```
- Use webcam:
  ```bash
  python detect.py --webcam
  ```

## Algorithm Overview
1. Read frame and convert to grayscale
2. Apply Gaussian blur to reduce noise
3. Use Canny edge detector to find edges
4. Mask the region of interest (polygon covering the lane area)
5. Use Hough transform to detect line segments
6. Separate left and right lanes based on slope and average them
7. Extrapolate lane lines and overlay them on the frame

## Tips for Improvements
- Improve robustness using perspective transform (bird's-eye view) and polynomial lane fitting
- Use color thresholding in HSV space to better pick lane markings
- Add Kalman filter / temporal smoothing across frames
- Replace with learning-based approaches (Segmentation networks) for difficult scenarios

## Dataset / Test Media
- Use dashcam images or public datasets like TuSimple, CULane, or KITTI for more thorough evaluation.

## Results and Evaluation
- Include example outputs in `out/` produced by running the scripts
- Report FPS for real-time processing on target hardware

## Folder Structure
- images/ - sample input images
- videos/ - sample input videos
- src/ - scripts (detect.py, helpers.py)
- out/ - output visualizations

## License
Specify license (e.g., MIT)

## Contact
GitHub: @chirravamshi
