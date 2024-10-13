# TP3: Fundamental Matrix
Syed Ali Haider | Computer Vision (Grad) with Prof. Jean Ponce
## Overview

This project was completed as part of my coursework, focusing on stereo vision and epipolar geometry. The primary objective was to compute the **Fundamental Matrix (F)** between two views using a set of 2D correspondences from the "house" dataset. The project also involved computing epipolar lines, estimating the Fundamental Matrix using the linear least-squares method, and improving the results using Hartley's normalization.

## Project Tasks

1. **Data Loading and Visualization**:
   - Loaded 2D image points for two views using custom functions.
   - Visualized the points and their corresponding edges for better understanding.

2. **Fundamental Matrix Calculation**:
   - Implemented the linear least-squares method to compute the Fundamental Matrix (F) using Singular Value Decomposition (SVD).
   - Enforced the rank-2 constraint on the computed matrix to ensure geometric consistency.

3. **Epipolar Geometry**:
   - Computed epipolar lines corresponding to the points in one view and plotted them over the second view to visualize their alignment.
   - Calculated the mean distance between the points and their corresponding epipolar lines.

4. **Hartley Normalization**:
   - Implemented Hartley's normalization technique to enhance the accuracy of the Fundamental Matrix estimation.
   - Re-calculated the Fundamental Matrix and observed significant improvement in the alignment of epipolar lines after normalization.
   - Reported the mean distance between points and epipolar lines after normalization, demonstrating reduced error.

5. **Epipolar Line Visualization**:
   - Visualized the epipolar lines before and after applying Hartley normalization.
   - Compared the results of the normalized and non-normalized Fundamental Matrices, showing a clearer and more accurate epipolar geometry post-normalization.

## Key Concepts

- **Fundamental Matrix (F)**: Encodes the epipolar geometry between two views, crucial for computing the epipolar lines across the two images.
- **Epipolar Lines**: The lines on which the corresponding point from one view should lie in the second view, based on the Fundamental Matrix.
- **Hartley Normalization**: A preprocessing step to improve numerical stability and accuracy in the estimation of the Fundamental Matrix.

## Results

The implementation successfully estimated the Fundamental Matrix, visualized epipolar lines, and demonstrated the improvements in stereo geometry using Hartley normalization. The reduction in the mean distance between points and their corresponding epipolar lines validated the effectiveness of normalization.
