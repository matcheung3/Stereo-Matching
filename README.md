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
├── CS4186_A2.ipynb # Main Jupyter Notebook containing the implementation
│
├── Art/
│ ├── view1.png     # Example stereo image (left)
│ ├── view5.png     # Example stereo image (right)
│ └── disp1.png     # Ground-truth disparity map
│
├── Dolls/
│ ├── view1.png     # Example stereo image (left)
│ ├── view5.png     # Example stereo image (right)
│ └── disp1.png     # Ground-truth disparity map
│
├── Reindeer/
│ ├── view1.png     # Example stereo image (left)
│ ├── view5.png     # Example stereo image (right)
│ └── disp1.png     # Ground-truth disparity map
│
└── README.md       # Project documentation
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

## 📊 Output

The computed disparity map will be displayed as an 8-bit grayscale image, and the PSNR score will indicate the similarity to the ground truth.
<img width="687" height="709" alt="image" src="https://github.com/user-attachments/assets/ea5a7646-6239-4976-ac56-b597f7042209" />
<img width="683" height="677" alt="image" src="https://github.com/user-attachments/assets/503d1fdf-8b70-4e20-b006-8f0bcaa4d603" />
<img width="684" height="670" alt="image" src="https://github.com/user-attachments/assets/5b359294-3341-449c-abbf-ce634d6a827d" />

---

## 👨‍💻 Author
This project was developed as part of **CS4186 - Computer Vision and Image Processing** coursework.
