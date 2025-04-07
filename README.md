# 🧠 Computer Vision Mini Project - Edge Detection

## 📌 Project Overview

This mini-project explores foundational concepts in computer vision including **corner detection** and **edge detection** techniques. The algorithms implemented help identify significant image features, such as corners and object boundaries.

---

## 🧪 Implemented Algorithms

### 1. 🧱 Harris Corner Detection
- Detects corners using intensity variations in both directions.
- 🔧 Parameters:
  - `blockSize`: Neighborhood size
  - `ksize`: Sobel kernel size
  - `k`: Harris detector free parameter (0.04–0.06 ideal)
- ✅ Used: `cv2.cornerHarris()`
- 🟥 Detected corners are marked in red.

---

### 2. 📌 Shi-Tomasi Corner Detection
- An improved version of Harris using minimum eigenvalue for better stability.
- 🎯 Common in tracking (e.g., Lucas-Kanade Optical Flow).
- 🔧 Parameters:
  - `qualityLevel`: Minimum accepted quality of corners.
  - `minDistance`: Minimum distance between detected corners.
- ✅ Used: `cv2.goodFeaturesToTrack()`
- 🔵 Corners plotted using colored dots.

---

### 3. ✂️ Canny Edge Detection
- Multi-stage algorithm to detect clear and connected edges.
- 🛠️ Steps:
  1. Noise reduction with Gaussian Blur
  2. Gradient calculation (Sobel)
  3. Non-maximum suppression
  4. Double thresholding and edge tracking by hysteresis
- ✅ Used: `cv2.Canny()`
- 🎯 Helps visualize object structure & boundaries.

---

## 🎓 Learnings & Insights

- Gained hands-on experience in **feature detection pipelines**.
- Understood how **parameter tuning** affects detection quality.
- Implemented real-world corner detection and **robust matching with RANSAC**.
- Explored practical applications of **homography** and **optical flow**.
