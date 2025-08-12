# CS4186 - Computer Vision and Image Processing  
## Assignment: Stereo Vision and Disparity Map Computation

This repository contains the implementation for a CS4186 undergraduate assignment on **Computer Vision and Image Processing**.  
The project focuses on **stereo vision** — computing disparity maps from stereo image pairs and evaluating results using the **Peak Signal-to-Noise Ratio (PSNR)** metric.

---

## 📜 Project Overview

The goal of this assignment is to:
- Load stereo image pairs (left and right images) along with ground-truth disparity maps.
- Apply **Gaussian filtering** to reduce image noise.
- Use OpenCV's `StereoSGBM` algorithm to compute disparity maps.
- Normalize results for visualization.
- Compare computed disparity maps against ground-truth data using PSNR.

---

## 📂 Repository Structure

```
.
├── CS4186_A2.ipynb         # Main Jupyter Notebook containing the implementation
├── images/                 # Example stereo images and ground truth disparity maps (if included)
└── README.md               # Project documentation
```

---

## ⚙️ Requirements

Before running the notebook, make sure you have Python 3.x installed and install the following dependencies:

```bash
pip install opencv-python numpy
```

---

## 🧮 Core Functions

### `compute_disparity_map(image_left, image_right, disp_gt)`
- **Inputs:**  
  - `image_left`: Path to left stereo image  
  - `image_right`: Path to right stereo image  
  - `disp_gt`: Path to ground-truth disparity map
- **Outputs:**  
  - `disp`: Normalized computed disparity map  
  - `psnr`: Peak Signal-to-Noise Ratio between computed and ground truth

---

## 📊 Example Output

The computed disparity map will be displayed as an 8-bit grayscale image, and the PSNR score will indicate the similarity to the ground truth.

---

## 👨‍💻 Author
This project was developed as part of **CS4186 - Computer Vision and Image Processing** coursework.
