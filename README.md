# backyard-ml

> Wildlife detection and video processing tools for multi-camera setups, optimized for edge devices and real-world backyards 🐿️📷

## Overview

This repo contains a set of modular tools and scripts to:
- Ingest and segment RTSP or video files
- Run object detection (e.g., squirrels, birds, cats) using OpenVINO and YOLOv8
- Sample, process, and visualize frames
- Support both real-time and offline pipelines

## Repo Structure

- `scripts/`: Command-line entry points for running detection, frame sampling, etc.
- `detector/`: Detection logic and post-processing for OpenVINO and YOLO models
- `ingest/`: RTSP and local video ingestion utilities
- `shared/`: Common helpers (video ops, timestamp tools, drawing)
- `config/`: Example config files for various deployment modes
- `notebooks/`: Jupyter notebooks for testing, visualization, or debugging
- `recordings/`: Folder for local video files (ignored by git)

## Setup

```bash
# Option 1: pip
pip install -r requirements.txt

# Option 2: conda
conda env create -f environment.yml
conda activate backyard-ml
