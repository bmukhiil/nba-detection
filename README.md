# NBA Detection

## Overview

This repo is a computer-vision project focused on projecting basketball video into a bird's-eye court view and tracking player movement over time. The pipeline combines player detection, court registration, homography, and trajectory rendering to create a cleaner tactical view from broadcast-style footage.

## Stack

- Python
- YOLOv5
- OpenCV
- ResNet-based court mapping
- NumPy / SciPy

## What I Built

- A workflow for detecting players from basketball footage
- Court registration and homography mapping into a top-down tactical board
- Trajectory visualization across frames
- Supporting utilities for model analysis and experiment iteration

## Why I Built It

Basketball footage is hard to analyze from a coaching or systems perspective when the camera angle is tilted and noisy. This project explores how to turn raw video into a more tactical representation that makes spacing, movement, and player tracking easier to study.

## Outcome

This is a strong applied computer-vision portfolio project because it combines detection, calibration, homography, and visualization in one pipeline. The public repo is intentionally trimmed to source code and supporting assets rather than large datasets, checkpoints, and generated videos.

## Notes On The Public Version

- Training datasets are not included
- Model checkpoints are not included
- Generated videos and large local experiment artifacts are not included
- The vendored `yolov5` source is kept because the pipeline imports it directly

## Run Locally

Install the Python dependencies, add your own model weights and input footage, and then run:

```bash
python bird_eye_video.py
```
