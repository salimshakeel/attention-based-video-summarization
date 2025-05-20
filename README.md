# Attention-based-video-summarization
## Feature Extraction for Video Summarization

This project provides a pipeline to extract deep features from fighter jet videos to be used as input for the [PGL-SUM](https://github.com/ok1zjf/PGL-SUM) video summarization model.

## 📌 Overview

The `generate_features.py` script:
- Load the video.
- Samples frames at a fixed FPS-15.
- Uses a pretrained **GoogLeNet** model to extract spatial features.
- Averages the spatial dimensions to produce a fixed-length feature vector per frame.
- Stores features in an `.h5` file, compatible with the **TVSum/SumMe** dataset format used by PGL-SUM.

---
## ⚙️ Requirements

- Python 3.8+
- PyTorch
- OpenCV
- NumPy
- h5py
- torchvision
Install dependencies:
```bash
pip install torch torchvision opencv-python numpy h5py
