
---
```
# LAB 12 – Segmentation Techniques

## Overview
This lab explores **image segmentation techniques** using Python and OpenCV. The goal is to understand how different methods separate foreground from background in an image and compare their effectiveness.

Segmentation methods covered:

- Global Thresholding
- Adaptive Thresholding (Mean & Gaussian)
- K-Means Clustering
- Mean Shift Segmentation

---

##  Objectives

1. Understand **image segmentation** concepts.
2. Apply **global, local, and adaptive thresholding** techniques.
3. Perform **K-Means clustering** with different cluster values (k = 2, 3, 4).
4. Apply **Mean Shift segmentation**.
5. Visually compare segmentation results.
6. Analyze strengths and limitations of each method.

---

## Image Requirements

Segmentation requires an input image. Best practices for selecting an image:

- Colored image (JPG or PNG)
- Clear distinction between foreground and background
- Moderate texture and contrast
- Examples: landscapes, road/building scenes, flowers, fruits, or objects

📁 Folder Structure:

```

Lab12_Segmentation/
│
├── input/
│   └── image.jpg
│
├── output/
│   ├── thresholding.png
│   ├── kmeans_k2.png
│   ├── kmeans_k3.png
│   ├── kmeans_k4.png
│   ├── meanshift.png
│   └── segmentation_comparison.png
│
└── lab12_segmentation.py

```

---

## Code
```
The complete, error‑free Python code for this lab is in `lab12_segmentation.py`.  
It includes:

- Loading the image
- Thresholding techniques (global & adaptive)
- K‑Means segmentation
- Mean Shift segmentation
- Visual comparison of results
- ```
## Output Files
```

| File | Description |
|------|-------------|
| thresholding.png | Global & adaptive thresholding results |
| kmeans_k2.png | K‑Means segmentation (k=2) |
| kmeans_k3.png | K‑Means segmentation (k=3) |
| kmeans_k4.png | K‑Means segmentation (k=4) |
| meanshift.png | Mean Shift segmentation result |
| segmentation_comparison.png
```

## Discussion
```

### 🔹 Global Thresholding
- Simple and fast
- Works well with uniform lighting
- ❌ Fails with uneven illumination

### 🔹 Adaptive Thresholding
- Handles varying lighting
- Better for real‑world images
- ❌ Higher computational cost

### 🔹 K‑Means Segmentation
- Color‑based clustering
- Easy to implement
- Choice of k affects quality

### 🔹 Mean Shift Segmentation
- Produces smooth, natural segments
- Does not require specifying k
- ❌ Computationally intensive
- ```


## Conclusion
```

This lab demonstrates multiple segmentation techniques and highlights their effectiveness under different image conditions.  
Adaptive thresholding and Mean Shift provide better results for complex images, while K‑Means gives controllable segmentation through cluster selection.
```

##  References
```

- OpenCV Documentation: https://docs.opencv.org  
- Gonzalez & Woods, *Digital Image Processing*
```
