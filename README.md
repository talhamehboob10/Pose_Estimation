# Pose_Estimation

## Motivation:
Mixed reality is the spatial alignment between the real world and virtual world. Physical and virtual objects may co-exist in mixed reality environments and interact in real time. At every given instance mixed reality systems needs to track user and real-world surroundings, to keep the illusion of “reality”. For tracking and spatial mapping of the real world objects, the multi modal sensor data is used and most of the existing techniques support the 'macro movements' generated from the head movement. But, there are limited techniques that focus on the 'micro movements' such as performing a surgery requiring micro level tracking of the hands. 

## Design Goals:
In this project, we want to develop a 3D pose estimation technique for micro-level tracking of hand movements. 

## Deliverables:
* Acquiring GPUs and setting up CUDA environment on a Shared Cluster (Unity Cluster). 
* Download the Data onto the Unity Cluster 
* Training the Select Fusion model for macro movements data 
* Select Testing macro movements data and test the model 
* Compare the output Trajectories with the ground truths and find the mean error  
* Repeat the training and testing of the Select Fusion Model with the 'Micro Movements Data' 
* Generate more micro movements data using the HoloLens (if required) 

Below tasks are low priority tasks for now and we'll do work 

* Research new algorithms (besides Select Fusion) which could work for multiple camera at a time (Select Fusion only works with one camera images at one time) 
* If possible, do the necessary changes in the video encoder section of Select Fusion to in-corporate depth images as well, this step could highly optimize the micro-movements tracking. 

## System Blocks: 


## HW / SW Requirements: 
* Microsoft HoloLens to generate more data on micro-movement tracking (if required) for the training purposes 
* A PC/Laptop with CUDA enabled GPUs or access to cloud resources with required GPUs 
* Programming Language: Python 

## Team: 
Talha would be working on this project alone and is responsible for software setup, algorithm design, research and writing the final report. 

## Project Timeline: 
![Timeline](https://user-images.githubusercontent.com/39377184/193309073-3ad02ca8-547e-4957-bb00-e33995d01dc0.png)


## References: 
* SelectFusion: A Generic Framework to Selectively Learn Multisensory Fusion (https://arxiv.org/ pdf/1912.13077.pdf)
* Learning to Fuse: A Deep Learning Approach to Visual-Inertial Camera Pose Estimation (https://ieeexplore.ieee.org/document/7781768)
* Robust Pose Estimation for Outdoor Mixed Reality with Sensor Fusion (https://link.springer.com/ content/pdf/10.1007/978-3-642-02713-0_30.pdf)
* OxIOD: The Dataset for Deep Inertial Odometry (https://arxiv.org/abs/1809.07491)
