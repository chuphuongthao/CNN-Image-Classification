# CNN-Image-Classification

## Overview
This project focuses on image classification using Convolutional Neural Networks (CNNs) in TensorFlow. The goal is to classify bird species using either the NABirds dataset or the Caltech-UCSD Birds-200-2011 (CUB 200) dataset. The project builds upon fundamental image classification techniques and explores the effectiveness of binary classifiers in distinguishing between similar bird species.

## Key  Objectives
- Utilize TensorFlow to classify images in Python.
- Implement a Convolutional Neural Network (CNN) for image classification.
- Interpret CNN results using TensorFlow visualization tools.
- Train multiple pre-trained binary classifiers to make predictions on a dataset.

## Datasets
Two well-known bird classification datasets:


| Dataset | Download Link | Filename | 
|---|---|---|
| CUB 200 | https://data.caltech.edu/records/65de6-vp158 | CUB_200_2011.tgz |
| NABirds | https://dl.allaboutbirds.org/nabirds | nabirds.tar.gz |

**Note: The NABirds dataset requires user registration and agreement to its terms before download.**

## Project Setup
1. Choose a Dataset
Both datasets contain images organized by bird species, but their structures differ slightly:

CUB 200: Folder names include a unique ID and species name.
NABirds: Uses a numeric folder system, requiring classes.txt for species lookup.

2. Install Dependencies
Ensure TensorFlow 2.10 is installed. Python 3.9 is recommended, as TensorFlow 2.10 does not support Python 3.10.

3. Prepare Image Data
The dataset must be structured for TensorFlow’s image_dataset_from_directory method:

```
> parent_folder
	> class_a_folder
		class_a_img_1.jpg
		class_a_img_2.jpg
		...
	> class_b_folder
		class_b_img_1.jpg
		class_b_img_2.jpg
		...
```

4. Train & Evaluate Binary Classifiers
The project involves selecting ten bird pairings and training a separate binary classifier for each. Before training, a hypothesis should be made regarding which pairs will be more difficult to classify.

Note: Predictions may not always align with initial hypotheses, providing insights into model performance.

## Next Steps
- Experiment with different CNN architectures to improve accuracy.
- Fine-tune models with additional preprocessing and augmentation techniques.
- Compare results between the two datasets to assess their effectiveness in training deep learning models.
