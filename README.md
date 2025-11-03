# Otsu Segmentation and Morphological Operations 

This project implements the Otsu thresholding segmentation method and morphological operations — including erosion, dilation, and opening — using pure Python, without any built-in image processing libraries.
It compares segmentation results before and after applying morphological processing to demonstrate how these operations improve image clarity and boundary definition.

## Features

1. Otsu’s Thresholding (manual implementation)
2. Binary Erosion, Dilation, and Opening
3. Comparison between raw Otsu and post-morphology results
4. Visualization of original image, binary mask, and histograms

## Tools Used

1. NumPy → matrix operations
2. PIL (Pillow) → image loading & grayscale conversion
3. Matplotlib → visualization
All segmentation and morphological operations are implemented manually, without using libraries such as OpenCV or scikit-image.

## Key Concepts

- Otsu Method: Automatically finds the optimal threshold separating foreground and background based on pixel intensity variance.
- Erosion: Removes small white noise and shrinks bright areas.
- Dilation: Expands bright regions and fills small gaps.
- Opening: Combination of erosion and dilation to clean noise while preserving shapes.

## Results

The notebook demonstrates that before applying morphological operations, the binary segmentation produced by the Otsu method still contains noticeable noise and rough edges, causing the object boundaries to appear uneven and fragmented. After applying morphology, the results show smoother object shapes, reduced background noise, and clearer separation between different regions, leading to a more refined and accurate segmentation outcome.

## Reference
1. How do I implement Otsu's thresholding in Python without using OpenCV and MATLAB? - https://www.quora.com/How-do-I-implement-Otsus-thresholding-in-Python-without-using-OpenCV-and-MATLAB-1
2. Otsu-Thresholding - https://github.com/mohabmes/Otsu-Thresholding
3. OpenCV Morphological Operations - Dilation and Erosion - https://www.youtube.com/watch?v=03B64y9jrF0
