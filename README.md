# Computer Vision Algorithms & Implementation

## 📚 Overview
This repository contains implementations of fundamental Computer Vision algorithms developed for the **ECE457** course (Fall 2025-2026). The project focuses on low-level image processing techniques, ranging from spatial domain filtering and binarization to frequency domain analysis and edge detection.

All implementations are done in **Python** using `NumPy`, `OpenCV`, and `Matplotlib`, with a strong emphasis on performance metrics (PSNR, Edge Density) and comparative analysis.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** NumPy, OpenCV (cv2), Matplotlib, SciPy
* **Tools:** Jupyter Notebooks

---

## 📂 Projects Breakdown

### Assignment 1: Image Enhancement & Segmentation

#### [Part 1: Image Binarization & Thresholding](./Assignment_1_Image_Enhancement/Part1_Binarization_Thresholding.ipynb)
Implemented manual and automated thresholding techniques to convert grayscale images into binary maps.
* **Key Techniques:** Global Thresholding, Otsu’s Method.
* **Analysis:** Analyzed pixel distribution to determine optimal separation points for foreground/background segmentation.

#### [Part 2: Noise Reduction & Filter Analysis](./Assignment_1_Image_Enhancement/Part2_Noise_Reduction_Filters.ipynb)
A comparative study of spatial filters for removing additive noise.
* **Filters Implemented:** Gaussian Filter, Box (Average) Filter, Median Filter.
* **Performance Metric:** Peak Signal-to-Noise Ratio (PSNR).
* **Key Findings:**
    * **Gaussian Filter** yielded a PSNR of **26.31 dB**, outperforming the Box filter (25.80 dB) for additive Gaussian noise.
    * **Median Filter** proved superior for removing "Salt-and-Pepper" impulsive noise by preserving edges while eliminating spikes.

---

### Assignment 2: Edge Detection & Frequency Domain

#### [Part 1: Spatial Edge Detectors](./Assignment_2_Edge_Detection/Part1_Spatial_Edge_Detectors/image1/assignment2_part1.ipynb)
Developed and compared various gradient-based edge detection operators.
* **Algorithms:** Sobel, Prewitt, Laplacian, and Canny Edge Detector.
* **Metric:** **Edge Density** (Ratio of edge pixels to total pixels).
* **Observations:** The **Canny detector** demonstrated the highest efficiency, producing thin, continuous edges with the lowest edge density compared to the thicker responses of Sobel and Prewitt.

#### [Part 2: Frequency Domain Filtering](./Assignment_2_Edge_Detection/Part2_Frequency_Domain_Filters/image1/Assignment2-part2.ipynb)
Explored image filtering in the frequency domain using Fourier Transforms (FFT).
* **Technique:** High-Pass Filtering (HPF) with varying radii (0.05, 0.12, 0.25).
* **Results:** demonstrated the inverse relationship between filter radius and edge density; larger radii (e.g., 0.25) acted as "stricter" filters, retaining only the sharpest structural outlines.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/Computer-Vision-ECE457.git](https://github.com/yourusername/Computer-Vision-ECE457.git)
