# STS Fatigue Analyzer

This repository contains the code and example reports for a Sit-to-Stand (STS) fatigue analysis system.  
The system uses MediaPipe Pose and a rule-based engine to compare fresh vs post-exercise STS movements and generate a one-page PDF report.

## Features

- Markerless pose estimation using MediaPipe Pose
- Automatic extraction of hip and knee joint angles from STS videos
- Time-series plots, knee and hip trajectories, and summary tables
- Dynamic Time Warping comparison between fresh and tired sessions
- Rule-based fatigue verdict (fatigue likely vs no strong fatigue signal)

## Requirements

- Python 3.10 (or your version)
- Jupyter Notebook
- Main Python packages  
  - `mediapipe`  
  - `opencv-python`  
  - `numpy`  
  - `pandas`  
  - `matplotlib`  
  - `dtw` (or the DTW package you used)

## How to run

1. Clone this repository
2. Install the required Python packages
3. Open `fyp2.ipynb` in Jupyter Notebook
4. Update the video file paths to your own **fresh** and **tired** STS recordings
5. Run all cells to generate the analysis and the PDF report under the `reports/` folder

## Repository structure

- `notebooks/` – Jupyter notebooks (eg. `fyp2.ipynb`)
- `src/` – Python scripts (if you split functions out)
- `data/` – Example STS videos or CSV files (small samples only)
- `reports/` – Example output STS performance reports in PDF format
- `README.md` – This file

## Acknowledgements

This work was developed as part of a Final Year Project on fatigue-related biomechanical changes in Sit-to-Stand performance.
