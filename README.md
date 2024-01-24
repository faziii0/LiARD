# LiARD+++
A Multi-Modal Feature Fusion Network for 3D Object Detection

# Code will be available Soon


![Fusion-new drawio](https://github.com/faziii0/LiARD/assets/111413133/bce1d434-21bc-4aa1-86ed-14e080e8d90f)

Environment:
Linux (tested on Ubuntu 22.04)
Python 3.8
PyTorch 1.10 + CUDA-11.3

# Clone Repo:
   git clone https://github.com/faziii0/LiARD

# Installation:
  1. conda create -n liard python==3.8
  2. conda activate liard
  3. conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cudatoolkit=11.3 -c pytorch -c conda-forge
  4. conda install -c conda-forge cudatoolkit-dev
  5. pip install -r requirements.txt
  6. sh build_and_install.sh

# Dataset preparation:
Please download the official KITTI 3D object detection dataset and  train mask from Epnet++

mkdir EPNetV2
cd EPNetV2
mkdir data lib pointnet2_lib tools
cd data
mkdir KITTI
cd KITTI
mkdir ImageSets object
cd object
mkdir training testing
cd training
mkdir calib velodyne label_2 image_2 planes train_mask
cd ../testing
mkdir calib velodyne image_2
cd ../../../../..

 ├── point_depth
 ├── tools


