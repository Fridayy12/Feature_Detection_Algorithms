# Feature_Detection_Algorithms
Implementation of SIFT, Harris Corner Detection, and RANSAC algorithms for image feature detection and matching using OpenCV in Python.

# Feature Detection Algorithms Documentation

## Project Overview
This project implements three fundamental computer vision algorithms for feature detection and matching using OpenCV in Python. The implementations are designed to run in VS Code with proper Python environment setup.

## Implemented Algorithms

### 1. SIFT (Scale-Invariant Feature Transform)
**File:** `sift_feature.py`  
**Purpose:** Detect and match keypoints between two images  
**Key Functions:**
- `cv2.SIFT_create()` - Creates SIFT detector
- `detectAndCompute()` - Finds keypoints and descriptors
- `BFMatcher()` - Brute-force feature matcher
- `drawMatchesKnn()` - Visualizes matched features

### 2. Harris Corner Detection
**File:** `harris_corner.py`  
**Purpose:** Identify and visualize corners in an image  
**Key Functions:
- `cv2.cornerHarris()` - Harris corner detector implementation
- `cv2.dilate()` - Enhances corner markers
- Thresholding - Identifies significant corners

### 3. RANSAC (Random Sample Consensus)
**File:** `ransac_matching.py`  
**Purpose:** Remove outlier matches and fit transformation model  
**Key Functions:
- `cv2.FlannBasedMatcher()` - Efficient feature matcher
- `cv2.findHomography()` - Computes transformation with RANSAC
- `cv2.drawMatches()` - Visualizes inlier matches
