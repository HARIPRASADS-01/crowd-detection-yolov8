# Crowd Detection Using YOLOv8

This project performs real-time crowd detection using the YOLOv8 model. It detects people in video frames and calculates the crowd count for each frame. The output includes a video with bounding boxes around detected people and a graph showing the number of people detected over time.

## Features

- Real-time person detection using YOLOv8.
- Outputs a video (`crowd_detected_output.avi`) with bounding boxes and crowd count per frame.
- Generates a crowd count graph (`crowd_count_graph.png`) showing the number of people detected in each frame.

## Getting Started

### Prerequisites

Ensure you have Python installed, and install the required dependencies using the `requirements.txt` file.

### Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/HARIPRASADS-01/crowd-detection-yolov8.git
    cd crowd-detection-yolov8
    ```

2. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3. **Download YOLOv8 Weights:**
   The code uses the YOLOv8n model. Ensure that you have the `yolov8n.pt` file downloaded, or modify the script to use a different YOLOv8 model.

   You can download it using:
    ```bash
    yolo download model=yolov8n.pt
    ```

### Usage

1. **Run the detection script:**
    Replace `'test.mp4'` in the script with the path to your video file and run the script:
    ```bash
    python crowd_detection.py
    ```

2. **View Results:**
    - The output video with bounding boxes will be saved as `crowd_detected_output.avi`.
    - A graph showing the crowd count across video frames will be saved as `crowd_count_graph.png`.

### File Structure

```bash
.
├── crowd_detection.py    # Main script to run crowd detection
├── test.mp4              # Example video (not included)
├── requirements.txt      # Required dependencies
├── README.md             # Project documentation
└── crowd_count_graph.png # Graph output (generated after running the script)
