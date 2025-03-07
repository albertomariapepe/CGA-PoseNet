# 📸 CGAPoseNet: Camera Pose Regression with 1d-Up Conformal Geometric Algebra 🌍📐

## Overview
Welcome to **CGAPoseNet**. This repository contains the code for **CGA-PoseNet**, a deep learning framework for **camera pose regression** leveraging **1d-Up Conformal Geometric Algebra (CGA)**.

### Why CGAPoseNet? 🤖📷
- **Geometry-Aware Predictions**: Works directly in **spherical space**, making it ideal for camera pose estimation.
- **End-to-End Learning**: No need for handcrafted feature engineering.
- **1D-Up CGA Representation**: Ensures a **compact & efficient** formulation of pose regression.
- **No Need for Point Clouds**: Achieves top-tier results **without** requiring additional scene information.

---

## CGA-PoseNet: Abstract
We introduce **CGA-PoseNet**, which uses the **1D-Up approach** to **Conformal Geometric Algebra (CGA)** to represent rotations and translations with a single mathematical object, the **motor**, for **camera pose regression**. 

We build upon **PoseNet**, a model that successfully predicts camera poses from small datasets of RGB frames. However, state-of-the-art methods often require **expensive tuning** to balance the **orientational** and **translational** components of the camera. This is usually done via **complex, ad-hoc loss functions** and, in some cases, requires **3D points** in addition to images.

Our approach **unifies the camera position and orientation** through the **motor**, enabling the network to search for a **single object** within a **well-behaved 4D space** with a **Euclidean signature**. This allows us to address **image-only datasets** efficiently with a simple **mean squared error (MSE)** loss function between the predicted and ground truth motors. We demonstrate that achieving **high-accuracy camera pose regression** is possible with a significantly **simpler problem formulation**. The **1D-Up approach to CGA** can effectively overcome the dichotomy between **translational and orientational components** in camera pose regression in a compact and elegant way.

---

## 📁 How to Run the Notebooks 🏃‍♂️💻
Both notebooks can be run **end-to-end** as long as you have the corresponding datasets specified by **"FOLDER"** on the mounted Drive.

### 📥 Download the Datasets 🌍📸
The datasets required for training and evaluation can be obtained from:

🔹 **Cambridge Landmarks Dataset** 📍🏛️  
[Download Here](https://www.repository.cam.ac.uk/handle/1810/251291)  

🔹 **7-Scenes Dataset** 🏠📷  
[Download Here](https://www.microsoft.com/en-us/research/project/rgb-d-dataset-7-scenes/)  

Alternatively, refer to **references [26] and [41]** in the paper.

---

## 📖 Citation 📚
If you find this work useful, please cite:

```bibtex
@article{pepe2023cga,
  title={CGA-PoseNet: Camera pose regression via a 1D-up approach to conformal geometric algebra},
  author={Pepe, Alberto and Lasenby, Joan},
  journal={arXiv preprint arXiv:2302.05211},
  year={2023}
}
```
