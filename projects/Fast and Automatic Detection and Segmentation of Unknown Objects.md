---
tags:
  - resources/reading
  - projects/anytraverse
---
> [!help] Resources
> - :luc_file: [PDF](../resources/Automatic-Det-Seg-Unknown-Objs_Kootstra.pdf)
> - [Link](https://www.diva-portal.org/smash/get/diva2:454633/FULLTEXT01.pdf)

---

> [!quote] Abstract
> This paper focuses on the fast and automatic detection and ==segmentation of unknown objects in unknown environments==. Many existing object detection and segmentation methods assume prior knowledge about the object or human interference. However, an autonomous system operating in the real world will often be confronted with previously unseen objects. To solve this problem, we propose a segmentation approach named Automatic Detection And Segmentation (ADAS). For the detection of objects, we use symmetry, one of the [Gestalt principles](https://www.interaction-design.org/literature/topics/gestalt-principles?srsltid=AfmBOooo5IEh4Zv4X0a_mUCY7xuJfV2OHeNYk3L_ZsAJsuyg93Bn_awh) for figure-ground segregation to detect salient objects in a scene. From the initial seed, the object is segmented by iteratively applying graph cuts. We base the segmentation on both 2D and 3D cues: color, depth, and plane information. Instead of using a standard grid-based representation of the image, we use [**Superpixels**](../resources/Superpixels.md). Besides being a more natural representation, the use of super pixels greatly *improves the processing time of the graph cuts*, and provides more noise-robust color and depth information. The results show that both the object-detection as well as the object-segmentation method are successful and outperform existing methods.

# Introduction

- Paper gives novel framework for fast and automatic detection of unknown objects for **robotic applications**.
- Employs a *bottom-up approach*.
- Humans pay *attention to objects*, not basic features like color, brightness, etc. *(objects :luc_arrow_right: configural features)*.
- Previous methods use basic features *(contrast-saliency model)*.

## Configural Features

- High-level features integrating different parts of an figure.
- Example: *Symmetry*
	- Symmetry highlights symmetrical configurations in the figure.
	- Ability to detect objects through symmetry supported by Gestalt Theory.
	- Gestalt Theory assumes symmetry to be one of the principles for *figure ground segregation*.

> **Figure Ground-Segregation:** Figure-ground segregation is a fundamental perceptual process in which the visual system distinguishes an object (the figure) from its background (the ground).

## Figure-Ground Segregation

- Computational cost depends on number of points in the graph.
- To reduce complexity, use **superpixels**.
	- Reduce number of points
	- Preserving important boundaries.
	- Provides more noise-robust color and depth info
- Previously, superpixels used to segment images using [graph cuts](../resources/Graph%20Cuts.md).

## Contributions

1. **Detection of unknown objects** in realistic environment using local symmetry
2. **Real-time segmentation of objects** by iteratively applying graph cuts.

# Automatic Detection and Segmentation (ADAS)

## Overview

- Consists two parts:
	- Object detection method
	- Segmentation method

---

> [!warning] Hold Up
> 
> Wait a bit before proceeding, it might not be worth it.
