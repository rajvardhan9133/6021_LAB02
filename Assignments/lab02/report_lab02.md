# Lab Report — Lab 02: MRI Noise Removal via Fourier Notch Filtering

## Overview

_1 sentence: What was the goal of this lab?_
The goal of this lab is to remove the noise from a corrupted MRI image using Fourier domian notch filter.
## Implementation

_1-2 sentences: Briefly describe the steps you performed to remove the noise, including the (row, col) positions of the noise spikes you found and the notch radius you used._
I reconstructed the corrupted MRI image from its k-space data, and then used the fourier magnitude spectrum to find the noise spikes. Next, I created a notch mask around each spike, and applied this mask to the k-space data. Finally, I reconstructed the filtered image using the inverse fourier transform.
## Results

_1-2 sentences: Describe how the filtered image compares to the corrupted one._
The filtered MRI image shows reduced diagonal stripe interference while preserving the main anatomical structures.