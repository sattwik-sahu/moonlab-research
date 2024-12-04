---
tags:
  - resources/dataset
  - area/offroad
---
# Authors

- **Abhinav Valada**
    - Email: [avalada@cs.uni-freiburg.de](mailto:avalada@cs.uni-freiburg.de)
    - Website: [http://deepscene.cs.uni-freiburg.de](http://deepscene.cs.uni-freiburg.de/)

---

# Description

This package includes:

1. **Original dataset**
2. **Adverse conditions subset**: Contains images captured in snow, low-lighting, glare, and motion blur.

## Dataset Overview

- **Training Set**: 230 images
- **Test Set**: 136 images

For the ISER'16 paper, each image in the training set was augmented 300×. For details on the augmentations, refer to the ISER'16 paper.

## Citation

If you use this dataset for research, please cite the following paper:

> **A. Valada, G. Oliveira, T. Brox, and W. Burgard**,  
> "Deep Multispectral Semantic Scene Understanding of Forested Environments using Multimodal Fusion,"  
> _The 2016 International Symposium on Experimental Robotics (ISER 2016)_,  
> Tokyo, Japan, October 2016.
> 
> [Paper Link](http://ais.informatik.uni-freiburg.de/publications/papers/valada16iser.pdf)

```bibtex
@inproceedings{valada16iser,
  author = {Abhinav Valada and Gabriel Oliveira and Thomas Brox and Wolfram Burgard},
  title = {Deep Multispectral Semantic Scene Understanding of Forested Environments using Multimodal Fusion},
  booktitle = {The 2016 International Symposium on Experimental Robotics (ISER 2016)},
  year = 2016,
  month = oct,
  url = {http://ais.informatik.uni-freiburg.de/publications/papers/valada16iser.pdf},
  address = {Tokyo, Japan}
}
```

---

# Dataset Details

The dataset contains multispectral and multimodal images. Each image corresponds to a specific view of the scene. Note that the images in this dataset are not of uniform dimensions and must be resized before use.

## Contents

Each of the **Training** and **Test** sets contains the following data:

| **Folder Name**   | **Description**                                                                                     |
| ----------------- | --------------------------------------------------------------------------------------------------- |
| `rgb`             | Standard RGB images                                                                                 |
| `rgb_grayscale`   | Grayscale version of the RGB images                                                                 |
| `depth_color`     | 3-channel colorized depth images (Anat Levin's colorization applied)                                |
| `depth_color_1ch` | 1-channel colorized depth images (Anat Levin's colorization applied)                                |
| `depth_gray`      | 1-channel depth images                                                                              |
| `evi_color`       | 3-channel colorized Enhanced Vegetation Index (modified Jet colormap applied)                       |
| `evi_gray`        | 1-channel Enhanced Vegetation Index images                                                          |
| `ndvi_color`      | 3-channel colorized Normalized Difference Vegetation Index (modified Jet colormap applied)          |
| `ndvi_float`      | Normalized Difference Vegetation Index images in floating-point                                     |
| `nir`             | Images captured with a Wratten 25A filter (Near-Infrared in Blue channel, red light in Red channel) |
| `nir_color`       | 3-channel colorized Near-Infrared images (modified Jet colormap applied)                            |
| `nir_color_jet`   | 3-channel colorized Near-Infrared images (standard Jet colormap applied)                            |
| `nir_gray`        | 1-channel Near-Infrared images                                                                      |
| `nrg`             | 3-channel NRG (Near-InfraRed, RED, GREEN) images                                                    |
| `GT_color`        | Ground truth masks for semantic segmentation (color representation for visualization)               |

---

## Semantic Segmentation Classes

Ground truth annotations (`GT_color`) use the following color representations for semantic segmentation:

|**Class**|**R**|**G**|**B**|**ID**|
|---|---|---|---|---|
|Void|-|-|-|0|
|Road|170|170|170|1|
|Grass|0|255|0|2|
|Vegetation|102|102|51|3|
|Tree|0|60|0|3|
|Sky|0|120|255|4|
|Obstacle|0|0|0|5|

> **Note**: For training, create an ID image by assigning each color to the corresponding class ID.

---

## Changelog

**08/02/2018**

- Fixed incorrect label for the Obstacle class in the test ground truth.
- Fixed incorrect ground truth for test image `b275-311` and replaced it with the correct version.
- Removed duplicate test image `b223-093`.

---

For any further queries, contact [Abhinav Valada](mailto:avalada@cs.uni-freiburg.de).
