
# LiARD+++

A Multi-Modal Feature Fusion Network for 3D Object Detection

# Code will be available Soon
########![Fusion-new drawio](https://github.com/faziii0/LiARD/assets/111413133/549191c3-7ab3-4c3a-8790-aeba81e0e851)

# Environment Setup:
Linux (tested on Ubuntu 22.04)

Python 3.8

PyTorch 1.10 + CUDA-11.3




## Installation:

To deploy this project run

```bash
git clone https://github.com/faziii0/LiARD
  
```

```bash
conda create -n liard python==3.8
conda activate liard
conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.cudatoolkit=11.3 -c pytorch -c conda-forge
conda install -c conda-forge cudatoolkit-dev
pip install -r requirements.txt
sh build_and_install.sh
```
## Dataset preparation:

Please download the official [KITTI 3D object detection](https://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=3d) dataset and  train mask from [Epnet++](https://github.com/happinesslz/EPNetV2)

```bash
LiARD
├── data
│   ├── KITTI
│   │   ├── ImageSets
│   │   ├── object
│   │   │   ├──training
│   │   │      ├──calib & velodyne & label_2 & image_2 & depth_image & train_mask
│   │   │   ├──testing
│   │   │      ├──calib & velodyne & image_2 & depth_image
├── lib
├── pointdep_lirad
├── tools
```
## Trained Model Evaluation





| Objects | Easy|Moderate     | Hard                   | 
| :-------- | :------- | :----------- | :----------|
| `Car` | 95.82% | 88.84% | 83.98%
| `Pedestrian` | 82.20% | 74.86% | 69.42%
| `Cyclist` | 84.99% | 70.30% | 67.10%

3D Predicted labels are avialable from the above Google


## Acknowledgements

 Thanks to all the contributors and authors of the project [PointRCNN](https://github.com/sshaoshuai/PointRCNN), [EPNet++](https://github.com/happinesslz/EPNetV2), [EPNet](https://github.com/happinesslz/EPNet)

## Citation



