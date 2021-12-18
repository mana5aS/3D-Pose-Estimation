# 3D-Pose-Estimation
This repository contains all the necessary files required to implement  3-D pose estimation using GANs.

## Overview
This project aims to generate visually intuitive 3 Dimensional Pose estimations for humans from 2D RGB images. Most 3D pose estimation solutions require the use of 3D datasets, and a method that can convert 2D images to 3D key joint positions using only a 2D dataset requires additional algorithms and methods to accomplish the task. We achieve this by breaking down our project into three intermediate steps, namely (i) 2D key-point generation, (ii) conversion of 2D to 3D poses using Generative Adversarial Networks (GANs), and (iii) rendering the generated 3D poses for visually informative results. 

## Dataset
The 2D image dataset used to train and test the model for our project was the MPII dataset, which is a state-of-the-art benchmark for evaluation of articulated human pose estimation. It consists of 25K images and contains over 40K humans performing over 400 different activities. This gives us a variety of images to train on, with one or multiple people in the frame, along with poses where joint positions overlap or are presented differently, allowing us to test the robustness of the GANs model.
The MPII dataset can be found ![here](http://human-pose.mpi-inf.mpg.de/#overview)

## Procedure
Perfom the following steps to implement the 3-D pose estimation:
#### 1. Download dataset
- Download the datasets from the Datasets folder uploaded here and store them in a folder locally or on a Google drive.
#### 2. Obtain 2-D joint locations using OpenPose
- Update the different file paths in Module1_OpenPose.ipynb according to where the datasets are stored.
- Run the colab notebook.
#### 3. Obtain 3-D human poses using GANs
- Update the different file paths in 3d_pose_estimation_GANs.ipynb according to where the datasets are stored.
- Run the colab notebook.

## Sample Result
<p>
    <img src="Results/img6_orig.png" width="300">
    <img src="Results/img6_2d.png" width="300">
    <img src="Results/img6_3d.png" width="200">
</p> 



