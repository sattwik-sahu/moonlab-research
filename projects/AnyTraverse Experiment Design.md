---
tags:
  - projects/anytraverse
  - resources/dataset
  - resources/experiments
---
# 📍 Locations

## IISER Bhopal

- Near *I ♥ IISERB* ^59f35d
- Construction sites
- Open grounds
- Hillside (offroad)

## Outside Campus

- [Thuna Nursery](https://maps.app.goo.gl/drvse4R6qBnSHVUY7) ^e3c2ce

---

# Experiments

## Traversibility

- *Add experiments*

## Negative Obstacles

- Find craters in [nursery](#^e3c2ce)
- Go to cliff near [IISERB Logo](#^59f35d)
- Find negative obstacles on campus
	- Stairs
	- Potholes
	- Off footpath

### Evaluating Results

- Can evaluate with better depth estimation using [Intel RealSense D435i RGB-D Camera](https://robu.in/product/intel-realsense-depth-camera-d435i/)
- Create custom **ground truths** for AnyTraverse.
	- Current GTs only for semantic segmentation, contain no information about actual traversibility of the region.
	- Need *information about traversibility* of regions in the image.
