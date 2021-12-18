# Notes: *UAV-based Forest Fire Detection and Localization Using Visual and Thermal Cameras*

## Abstract

* locating & detecting

* fire detection & navigation

* 2 kinds of images are aligned.

* The 2DOF frame to describe the UAV motion and test the fire detection algorithm.

* The UAV flies along the predefined path $\rightarrow$ possible fires $\rightarrow$ alarm and fly over the fire.

**Notes:** Can change the predefined path to an automatically generated path?

## Contents

1. Introduction
2. Literature review
   1. General methods for UAV-based forest fire detection.
   2. Use of visual, infrared and thermal cameras.
   3. Contribution of this work.

3. System components
   1. Raspberry + Visual + Thermal  + Python
   2. 2DOF frame

4. Fire Detection and Localization Algorithms
   1. Knowledge
   2. thermal sensor
   3. Fire detection algorithm
   4. Visual camera algorithm

5. Platform



## 4. Fire Detection and Localization Algorithm

* segmentation: *extract the possible features from an images*
* color can be expressed in many different ways which are called color space.

### Visual camera algorithm

* color threshold --- color based 
* motion features --- motion based



## 4.3.3 Visual & Thermal Image Fusion

formula 4.7, can't tell where it comes from.

x,y in the formula 4.10 are not defined.

## 4.4 Image-based thermo-visual servoing by 2DOF frame

* position-based visual servoing (PBVS) and image-based visual servoing (IBVS)
* Figure3.9 says it's open loop?!
* control law e_dot  = K*e