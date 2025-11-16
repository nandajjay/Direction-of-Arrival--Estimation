# DOA Estimation & Source Tracking

This repository implements DOA estimation using GCC-PHAT and MUSIC, with a Kalman filter-based tracker.
It includes:
- Room + array simulator (pyroomacoustics)
- GCC-PHAT and MUSIC implementations
- Angular Kalman filter for tracking
- Evaluation scripts and visualizations
- Demo audio files and animated plots

## How to run
1. `pip install -r requirements.txt`
2. `python src/simulate.py`  # generate demo data
3. `python src/run_experiment.py`  # runs DOA + tracking and produces plots

## Highlights
- Polar plot of true vs estimated track
- Mean DOA error, CDF plots
- Beamformed audio demo using estimated DOA
🎧 Real-Time Direction-of-Arrival Estimation & Acoustic Source Tracking
GCC-PHAT + MUSIC + Kalman Filter | Microphone Array Signal Processing
📌 Overview

This project implements a real-time (or offline) acoustic Direction-of-Arrival (DoA) estimation and source tracking system using microphone array signals.
It combines three powerful techniques:

GCC-PHAT → Robust Time Difference of Arrival (TDOA) Estimation

MUSIC Algorithm → High-resolution subspace-based DoA estimation

Kalman Filter → Smooth, stable tracking of moving sound sources

This pipeline models real engineering systems used in:
🎤 smart speakers,
🎧 gaming headsets,
📹 camera/audio tracking,
🏢 conference microphone arrays,
📱 spatial audio products.

🚀 Features

✔ Multi-microphone array processing (linear / circular / custom geometries)
✔ STFT-based pre-processing + noise reduction
✔ GCC-PHAT TDOA extraction
✔ MUSIC pseudo-spectrum computation
✔ DoA peak detection with subspace decomposition
✔ Continuous source tracking with Kalman filtering
✔ Real-time mode using PyAudio / sounddevice (optional)
✔ Visualizations: polar plots + 2D trajectory tracking
✔ Works with simulated or real recordings (.wav)

🛠️ Tech Stack

Python: NumPy, SciPy, Matplotlib

Optional: PyAudio/sounddevice for streaming

OR MATLAB equivalent scripts

No deep learning required — purely signal processing + numerical methods.
