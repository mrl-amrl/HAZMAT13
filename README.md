# Hazardous-Materials-HAZMAT-Sign-dataset

<!-- vscode-markdown-toc -->
**Table of content:**

* [Abstract](#Abstract)
* [1. Original model:](#Originalmodel:)
	* [Download:](#Download:)
* [2. Augmented model:](#Augmentedmodel:)
	* [Download:](#Download:-1)
* [3. Different distance](#Differentdistance)
	* [Download:](#Download:-1)
* [Citation](#Citation)

<!-- vscode-markdown-toc-config
	numbering=false
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->




---
## <a name='Abstract'></a>Abstract


We have developed a comprehensive dataset of HAZMAT sign, including images from various viewing angels, distortions, and different illumination conditions. The dataset has been divided into 13 different classes as shown below. The dataset is annotated with PASCAL-VOC format as it is easy to convert into other annotation formats such as YOLO or COCO.

| 1- Poison | <img src="images/classes/1-poison.png" alt="1-poison" width="100"/> | 2- Oxygen |<img src="images/classes/2-oxygen.png" alt="2-oxygen" width="100"/> |
|---|---|---|---|
| 3- Flammable Gas | <img src="images/classes/3-flammable-gas.png" alt="3-flammable-gas" width="100"/> | 4- Flammable Solid |<img src="images/classes/4-flammable-solid.png" alt="4-flammable-solid" width="100"/> | 
| 5- Corrosive |<img src="images/classes/5-corrosive.png" alt="5-corrosive" width="100"/> | 6- Dangerous | <img src="images/classes/6-dangerous.png" alt="6-dangerous" width="100"/> | 
| 7- Non-flammable Gas |<img src="images/classes/7-non-flammable-gas.png" alt="7-non-flammable-gas" width="100"/> | 8- Organic Peroxide | <img src="images/classes/8-organic-peroxide.png" alt="8-organic-peroxide" width="100"/> |
| 9- Explosive | <img src="images/classes/9-explosive.png" alt="9-explosive" width="100"/> |  10- Radioactive | <img src="images/classes/10-radio-active.png" alt="10-radio-active" width="100"/> |
| 11- Inhalation Hazard | <img src="images/classes/11-inhalation-hazard.png" alt="11-inhalation-hazard" width="100"/> | 12- Spontaneously Combustible | <img src="images/classes/12-spontaneously-combustible.png" alt="12-spontaneously-combustible" width="100"/>  | 
| 13- Infectious Substance | <img src="images/classes/13-infectious-substance.png" alt="13-infectious-substance" width="100"/>   |  |  |


The dataset consist of three different models that mentioned below: 
1. [1. Original model:](#Originalmodel:)
2. [2. Augmented model:](#Augmentedmodel:)
3. [3. Different distance](#Differentdistance)

---
## <a name='Originalmodel:'></a>1. Original model: 

Consist of 1685 images with no augment and consist of bounding box and segmented mask

<img src="images/samples.jpg" alt="13-infectious-substance" /> 
1. Row a, b: Samples in different angles, lighting conditions, and backgrounds. 
2. Row c , d: Samples in different situation at RoboCup competitions in past years.

### <a name='Download:'></a>Download:


[Download Link](https://drive.google.com/drive/folders/1-dQPRdQ-MRp6mrPhnpng5pcgJsTZMg23?usp=sharing)

---
## <a name='Augmentedmodel:'></a>2. Augmented model: 


Applying data augmentation we increased the number of HAZMAT signs to improve the performance of our algorithm. Besides, the dataset needs to be balanced and the number of images for each class should be almost same to have a Homogeneous dataset. Also, the size of our dataset should neither be very small that lead to model under-fitting and detection accuracy loss, and nor too large to increase the complexity of the feature extraction and overfitting challenges. To aim this, and using the augmentation technique, we expanded the dataset to 4065 images per class and in overall 52845 images. We split the dataset into 80% train set and 20% test set.


### <a name='Download:-1'></a>Download:

[Download Link](https://drive.google.com/drive/folders/1ZglTZkiIhb6xI0v9cwXJfV2-Y4yL9S1V?usp=sharing)

---

## <a name='Differentdistance'></a>3. Different distance
We prepare small dataset in 3 different distance to measure our method performance. It consist in 3 different distances 50cm, 100cm and 150cm.

|| 50cm | 100cm | 150cm |
|---|---|---|---|
|1 |<img src="images/DifferentDistances/50/01.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/01.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/01.jpg" alt="13-infectious-substance" width="100"/> |
|2 |<img src="images/DifferentDistances/50/02.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/02.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/02.jpg" alt="13-infectious-substance" width="100"/> |
|3 |<img src="images/DifferentDistances/50/03.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/03.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/03.jpg" alt="13-infectious-substance" width="100"/> |
|4 |<img src="images/DifferentDistances/50/04.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/04.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/04.jpg" alt="13-infectious-substance" width="100"/> |
|5 |<img src="images/DifferentDistances/50/05.jpg" alt="13-infectious-substance" width="100"/> |<img src="images/DifferentDistances/100/05.jpg" alt="13-infectious-substance" width="100"/>| <img src="images/DifferentDistances/150/05.jpg" alt="13-infectious-substance" width="100"/> |

### <a name='Download:-1'></a>Download:

[Download Link](https://drive.google.com/drive/folders/1aBcR-5jOs3gRce4oHBA1bQ3crp8F9UD-?usp=sharing)

---
## <a name='Citation'></a>Citation 
If this dataset help you during  research feel free to cite it:
```
@article{sharifi2020deephazmat,
  title={DeepHAZMAT: Hazardous materials sign detection and segmentation with restricted computational resources},
  author={Sharifi, Amir and Zibaei, Ahmadreza and Rezaei, Mahdi},
  journal={Available at SSRN 3649600},
  year={2020}
}
```