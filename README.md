# Awesome-Autonomous-Medical-Ultrasound-System
In this repository, we will collect and document startup companies, researchers, and their outstanding work related to autonomous medical ultrasound systems.

## Content

### Survey

- **Robotic ultrasound imaging: State-of-the-art and future perspectives,** Medical Image Analysis (2023.10).

  *Zhongliang Jiang, Septimiu E. Salcudean, Nassir Navab.* [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S136184152300138X)][Code]

### Cardiac

#### Datasets

- **Video-based AI for beat-to-beat assessment of cardiac function,** Nature (2020). ![](https://img.shields.io/badge/EchoNet_Dynamic-blue) ![](https://img.shields.io/badge/A4C_Left_Ventricle_Segmentation-green)

  *David Ouyang, Bryan He, Amirata Ghorbani, Neal Yuan, Joseph Ebinger, Curt P. Langlotz, Paul A. Heidenreich, Robert A. Harrington, David H. Liang, Euan A. Ashley, and James Y. Zou.* [[Dataset](https://echonet.github.io/dynamic/)][[Paper](https://www.nature.com/articles/s41586-020-2145-8)][[Code](https://github.com/echonet/dynamic)]

  **Description**: The dataset contains 10,030 apical-4-chamber echocardiography videos from individuals who underwent imaging between 2016 and 2018 as part of routine clinical care at Stanford University Hospital. Each video was cropped and masked to remove text and information outside of the scanning sector. The resulting images were then downsampled by cubic interpolation into standardized 112x112 pixel videos.

#### Probe Guidance

- **Straight to the point: reinforcement learning for user guidance in ultrasound,** arXiv:1903.00586 (2019). ![](https://img.shields.io/badge/PLAX_Plane-green)

  *Fausto Milletari, Vighnesh Birodkar, Michal Sofka.* [[Paper](https://arxiv.org/abs/1903.00586)][Code]
  
  - **Method**: deep reinforcement learning with simulated training environment by collecting ultrasound image and probe posture pairs from 7x7 spatial bins on patients' chest. The rotations and tilts are only collected in the bin marked as "correct" due to the huge time cost for collecting in all bins.
  - **Data**: train on 22 different environment with ~160,000 images and test on 5 different environment with ~40,000 images.
  - **Criteria**: whether provide the correct guidance towards the target bin; this criteria might be proper for the topic of probe guidance, but not suitable for autonomous plane localization.
  - **Experiments**: totally conducted in the offline environments; since the simulated environment is a simplified version of the situation in real world, it is not clear the performance when applied to real world.
  
### End-to-end Autonomous Ultrasound System

### Imaging

#### Image Enhancement

#### 3D Reconstruction from 2D Images

### Probe Navigation or Guidance

### Analysis and Diagnosis

### Foundation Model

- **USFM: A Universal Ultrasound Foundation Model Generalized to Tasks and Organs towards Label Efficient Image Analysis,** arXiv 2024 (arXiv:2401.00153). ![](https://img.shields.io/badge/USFM-blue) ![](https://img.shields.io/badge/Classification_,_Segmentation_,_Enhancement-green)

  *Jing Jiao, Jin Zhou, Xiaokang Li, Menghua Xia, Yi Huang, Lihong Huang, Na Wang, Xiaofan Zhang, Shichong Zhou, Yuanyuan Wang, Yi Guo.* [[Paper](https://arxiv.org/abs/2401.00153)][[Code](https://github.com/openmedlab/USFM)]

  **Insights**: the information in frequence domain may be a good way to distinguish similar ultrasound images as shown in Fig.1(c).
