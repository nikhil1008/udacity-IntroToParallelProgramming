# udacity-IntroToParallelProgramming
CS344 - Introduction To Parallel Programming course (Udacity) proposed solutions

Testing Environment: Visual Studio 2015 x64 + nVidia CUDA 8.0 + OpenCV 3.2.0

For each problem set, the core of the algorithm to be implemented is located in the _students_func.cu_ file.

## Problem Set 1 - RGB2Gray: 
### Objective
Convert an input RGBA image into grayscale version (ignoring the A channel).
### Topics
Example of a **map** primitive operation on a data structure.

## Problem Set 2 - Blur
### Objective
Apply a Gaussian blur convolution filter to an input RGBA image (blur each channel independently, ignoring the A channel).
### Topics
Example of a **stencil** primitive operation on a 2D array. Use of the **shared memory** in order to speed-up the algorithm. Both global memory and shared memory based kernels are provided, the latter providing approx. 1.6 speedup over the first.

## Problem Set 3 -Tone Mapping
### Objective
Map a High Dynamic Range image into an image for a device supporting a smaller range of intensity values.
## Topics
- Compute range of intensity values of the input image: min and max **reduce** implemented.
- Compute **histogram** of intensity values (1024-values array)
- Compute the cumulative ditribution function of the histogram: Hillis & Steele **scan** algorithm (step-efficient, well suited for small arrays like the histogram one). 

