---
tags:
  - resources/robotics
  - projects/dl-rl
  - resources/components
---
# Manipulators

1. [Open Manipulator-X](https://emanual.robotis.com/docs/en/platform/openmanipulator_x/overview/)
2. [Trossen Robotics ViperX 300S](https://www.trossenrobotics.com/viperx-300)

# Peripherals

1. [Hand Motion Sensor](https://www.desertcart.in/products/652515531-robot-hand-glove-control-gesture-sensing-for-arduino-robot-open-source-wireless-somatosensory-mechanical-robot-arm-glove-for-robot-secondary-development) for data collection

---

# Open Manipulator-X

## Buy Here

| Link                                                                                                                                      | Price (Rs.) |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| [MG Super Labs](https://www.mgsuperlabs.co.in/estore/RM-X52-TNM-OpenManipulator-X)                                                        | `1 58 000`  |
| [Open Manipulator](https://www.robotis.us/openmanipulator-x-rm-x52-tnm/?srsltid=AfmBOopzA6EXWvWdY_Sc1YtcZkrTYvopHAIGq2R96BF6cXuWNCEpIhm1) | `1 20 167`  |

## Specifications

- [Website](https://emanual.robotis.com/docs/en/platform/openmanipulator_x/specification/#hardware-specification)
- **Degrees of Freedom:** 5 (4 + 1 DOF Gripper)
- **Max Payload:** 500 g
- **Weight:** 700 g

## Integrations

### Software

- MoveIt! ROS package
- Gazebo Simulation available

### Hardware

- [OpenCR](https://emanual.robotis.com/docs/en/parts/controller/opencr10/): Open Source Control Module for ROS 🤔 *(Nice, ig?)*

## Getting Started

- **Embedded Systems:** OpenCR + PC
- **With ROS:** [Dynamixel Starter Set](https://www.robotis.us/dynamixel-starter-set-us/?srsltid=AfmBOoqbcY3vu_SbjoMiO3ERLIka89IqgnoOEVT7cJh1XcLAz8-yJZsy) or OpenCR

## Accessibility

- `.stl` files available on web. Components can be 3D printed. *Broken components can be replaced easily*.

> [!info] Extra Resources
> - [Example video](https://youtu.be/B2pnXtooKOg)

---

# Trossen Robotics ViperX 300S

## Buy Here

| Link                                                           | Price      |
| -------------------------------------------------------------- | ---------- |
| [Trossen Robotics](https://www.trossenrobotics.com/viperx-300) | `5 20 000` |

## Specifications

- **Degrees of Freedom:** 6
- **Max Payload:** 750 g
- **Weight:** 3.6 kg

## Integration

### Hardware

- Link to [3D CAD files](https://drive.google.com/drive/folders/1mhJuhzT4lBnvZ9VE57UgT6vmJDFPVsBf)

### Software

- Full ROS and ROS2 supported
- Gazebo supported
	- URDF provided in package
	- Meshes provided along with accurate inertial models
- MoveIt! ROS package supported

## Accessibility

- 3D printed end effectors
- Motors can be swapped if broken

> [!info] Extra Resources
> - [Setup tutorial video](https://youtu.be/o9EXEgzbAxQ)
