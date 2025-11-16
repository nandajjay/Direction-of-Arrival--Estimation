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
