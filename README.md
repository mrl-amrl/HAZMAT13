### HAZMAT-13: Hazaradous Materials Signs Dataset

---
#### Abstract

We have developed a comprehensive dataset of HAZMAT sign, including images from various viewing angels, distortions, and different illumination conditions. The dataset has been divided into 13 different classes as shown below. The dataset is annotated with PASCAL-VOC format as it is easy to convert into other annotation formats such as YOLO or COCO.

| Name | Image | Name | Image |
|---|---|---|---|
| 1- Poison | <img src="images/classes/1-poison.png" alt="1-poison" width="100"/> | 2- Oxygen |<img src="images/classes/2-oxygen.png" alt="2-oxygen" width="100"/> |
| 3- Flammable Gas | <img src="images/classes/3-flammable-gas.png" alt="3-flammable-gas" width="100"/> | 4- Flammable Solid |<img src="images/classes/4-flammable-solid.png" alt="4-flammable-solid" width="100"/> | 
| 5- Corrosive |<img src="images/classes/5-corrosive.png" alt="5-corrosive" width="100"/> | 6- Dangerous | <img src="images/classes/6-dangerous.png" alt="6-dangerous" width="100"/> | 
| 7- Non-flammable Gas |<img src="images/classes/7-non-flammable-gas.png" alt="7-non-flammable-gas" width="100"/> | 8- Organic Peroxide | <img src="images/classes/8-organic-peroxide.png" alt="8-organic-peroxide" width="100"/> |
| 9- Explosive | <img src="images/classes/9-explosive.png" alt="9-explosive" width="100"/> |  10- Radioactive | <img src="images/classes/10-radio-active.png" alt="10-radio-active" width="100"/> |
| 11- Inhalation Hazard | <img src="images/classes/11-inhalation-hazard.png" alt="11-inhalation-hazard" width="100"/> | 12- Spontaneously Combustible | <img src="images/classes/12-spontaneously-combustible.png" alt="12-spontaneously-combustible" width="100"/>  | 
| 13- Infectious Substance | <img src="images/classes/13-infectious-substance.png" alt="13-infectious-substance" width="100"/>   |  |  |


The dataset consist of three different models that mentioned below: 

---
#### 1. Original model: 

Consist of 1685 images with no augment and consist of bounding box and segmented mask

<img src="images/samples.jpg" alt="13-infectious-substance" /> 

1. Row a, b: Samples in different angles, lighting conditions, and backgrounds. 
2. Row c, d: Samples in different situation at RoboCup competitions in past years.

[Download Link](https://drive.google.com/drive/folders/1-dQPRdQ-MRp6mrPhnpng5pcgJsTZMg23?usp=sharing)

---
#### 2. Augmented model: 

Applying data augmentation we increased the number of HAZMAT signs to improve the performance of our algorithm. Besides, the dataset needs to be balanced and the number of images for each class should be almost same to have a Homogeneous dataset. Also, the size of our dataset should neither be very small that lead to model under-fitting and detection accuracy loss, and nor too large to increase the complexity of the feature extraction and overfitting challenges. To aim this, and using the augmentation technique, we expanded the dataset to 4065 images per class and in overall 52845 images. We split the dataset into 80% train set and 20% test set.

[Download Link](https://drive.google.com/drive/folders/1ZglTZkiIhb6xI0v9cwXJfV2-Y4yL9S1V?usp=sharing)

---

#### 3. Different distance
We prepare small dataset in 3 different distance to measure our method performance. It consist in 3 different distances 50cm, 100cm and 150cm.

|| 50cm | 100cm | 150cm |
|---|---|---|---|
|1 |<img src="images/DifferentDistances/50/01.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/01.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/01.jpg" alt="13-infectious-substance" width="100"/> |
|2 |<img src="images/DifferentDistances/50/02.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/02.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/02.jpg" alt="13-infectious-substance" width="100"/> |
|3 |<img src="images/DifferentDistances/50/03.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/03.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/03.jpg" alt="13-infectious-substance" width="100"/> |
|4 |<img src="images/DifferentDistances/50/04.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/04.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/04.jpg" alt="13-infectious-substance" width="100"/> |
|5 |<img src="images/DifferentDistances/50/05.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/05.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/05.jpg" alt="13-infectious-substance" width="100"/> |

[Download Link](https://drive.google.com/drive/folders/1aBcR-5jOs3gRce4oHBA1bQ3crp8F9UD-?usp=sharing)

---
#### Citation 
If this dataset help you during  research feel free to cite it:
```
@article{SHARIFI2021100104,
title = {A deep learning based hazardous materials (HAZMAT) sign detection robot with restricted computational resources},
journal = {Machine Learning with Applications},
pages = {100104},
year = {2021},
issn = {2666-8270},
doi = {https://doi.org/10.1016/j.mlwa.2021.100104},
url = {https://www.sciencedirect.com/science/article/pii/S2666827021000529},
author = {Amir Sharifi and Ahmadreza Zibaei and Mahdi Rezaei},
keywords = {Hazardous materials, Object recognition, HAZMAT sign detection, Segmentation, CNN, Rescue robotics},
abstract = {One of the most challenging and non-trivial tasks in robot-based rescue operations is the Hazardous Materials (HAZMAT) sign detection in dangerous operation fields, in order to prevent further unexpected disasters. Each HAZMAT sign has a specific meaning that the rescue robot should detect and interpret it to take a safe action, accordingly. Accurate HAZMAT detection and real-time processing are the two most important factors in such robotics applications. Furthermore, the rescue robot should cope with some secondary challenges such as image distortion and restricted CPU and computational resources, embedded in the robot. In this research, we propose a CNN-Based pipeline called DeepHAZMAT for HAZMAT sign detection and segmentation in four steps: (1) Input data volume optimisation before feeding into the CNN network, (2) Application of a YOLO-based structure to collect the required visual information from the hazardous areas, (3) HAZMAT sign segmentation and separation from the background using adaptive GrabCut technique, and (4) Post-processing optimisation using morphological operators and convex hull algorithms. In spite of the utilisation of a very limited CPU and memory resources, the experimental results show the proposed method has successfully maintained a better performance in terms of detection-speed and detection-accuracy, compared to classical and modern state-of-the-art methods.}
}
```
