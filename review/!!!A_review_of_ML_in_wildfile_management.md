Review/!!!A_review_of_ML_in_wildfile_management ML methods in wildfire management
==================================================================================

**NOTE** section 3 is not full of information.

## Abstract

- **6 domains**
1. fuels(可燃物), fire detection, mapping
2. fire -> weather, climate change
3. fire occurrence, susceptibility, and risk
4. behavior prediction
5. fire effects
6. fire managements


- methods:
- Classic:
- [x] random forest
- [ ] MaxEnt
- [x] AN
- [x] SVM
- [x] DT decision tree
- [ ] GA 遗传算法
- Current:
- [x] Deep learning
- [ ] agent based learning

![methods](.\table_of_method_and_papers.png)

- Data features: very large multivariate data sets.

## 1 Introduction

  - The effect and process of wildfire
- The model of the wildfire(physical model)
  - combustion and ignition(physical model) is limited by the data(the amount
      and the quality) and computational power.
  - There are also "significant adcvances":
  - Satellites
  - ML

## 2 The ML and AI

  - supervised learning:
  The input and output are known, labeled data.

  - unsupervised learning
  The canonical tasks are dimensionality reduction and clustering.

  - agent-based learning
  Model learning by simulating behaviors and interactions of a signal or a group
  of autonomous agents.
  A specific case is the Reinforcement Learning.

### Decision Tree(DT)

  <font color=red>IDEA:</font> Hossian's work uses the man-made threshold to judje
  the color space, while we can use the DT to find the threshold automatically.

#### Random Forest
  bagged decision tree

#### Boosted Ensembles
  Faster, but not better than the DNNs

### SVM

### ANN and Deep Learning

  - ANN
  - DNN
  - CNN
  - RNN
  - SOM:
  ANN can also be configured doe unsupervised learning tasks.

### Bayesian methods

#### Bayesian Network

#### Naive Bayesian
  a special case of BN.

#### MaxEnt(Maximum Entropy)

### Reward based methods

#### Genetic Algorithms(GA)

#### Reinforcement Learning(RL)

### Clustering Methods

  - K-means etc.

### Others

#### KNN

#### Neuro-Fuzzy models

## 3 Literature search and scoping review

## 4 Wildfire applications

### 4.1 Fuels Characterization, Fire Detection and Mapping

#### 4.1.1 Fuels characterization

  Research to predict fuel prorerties.

  1. Regression to predict the quantities
  2. Air images $\rightarrow$ classification of the fuels.

#### 4.1.2 Fire detection

  1. <font color=red>IDEA:</font> can the small fire be detected?

  **what have been done:**

  - Traditional:
  - ANN+infrared(IR) 2000
  - multi-attributes of fire detection(flame, heat, light and radiation) 2015
  - SVM+Video 2011
  - GA+LiDAR-based 2004
  - BN+vision 2010

  - Modern:
  - CNN 2016, 2018, 2019
  - YOLO
  - CNN+optical flow
  - * 3D-CNN + both spatial and temporal information: smoke detection ==>
  segmentation
  - Convolutional layers + Long Short Term Memory(LSTM) 2019

#### Fire perimeter and severity mapping

  - <font color="red">IDEA:</font> Fire map, not only "yes" or "no".
  - <font color="red">IDEA:</font> Mainly for the burned area, not in progress,
  which is what we concern.

  1. map of the perimeter of fire
  2. map for the final burn perimeter and fire severity.

  **For burn mapping**
  - LR+ANN burn area mapping 2004
  - SVM, or K-nearest neighbour and K-means
  - FNC, SVM, AdaBoost 2012
  - SVM+feature selection methods(based on the fuzzy logic)==fast R-cnn 2014
  - ANN+MODIS hotspot data 2011
  - 3 stages framework for burned area mapping using MODIS data and ANN

  **For the burn severity:**
  - RF
  - MaxEnt
  - ...
- DNN+MODIS(光谱成像, like NVID and surface reflectance)
  - XGBoost

### 4.2 Fire Weather and Climate Change

### 4.3 Fire Occurrence, Susceptibility and Risk

#### 4.3.1 Fire occurrence prediction
#### 4.3.2 Landscape scale burned area prediction
#### 4.3.3 Fire Susceptibility Mapping
  map the wildfire susceptibility, coresponding to either the spatial probability
  or density of the fire occurrence.
#### 4.3.4 Landscape control on fire

### 4.4 Fire Behavior Prediction
  fire spread rates, fire growth, burned area, and fire severity, but it is on the
  prognostic application.

#### 4.4.1 Fire spread and growth

  - Physical-Model or quasi-physical nature.
  - ML methods for the fire growth
  - GA to optimize input params

  - ANN+Kalman Filter for data assimilation(同化) 2013
  - CA(a cellular automata) model + Extreme Learning Machine (ELM, a type of
      feedforward ANN)

#### 4.4.2 Burned area and fire severity prediction
predict the final area burned from a wildfire.
