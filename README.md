# Image Classification Model for Android BinBuddy App

## Overview
This project is part of the Bangkit Batch 2 2024 program, where we developed an **image classification model** used by the **Android BinBuddy app**. The goal of the model is to classify garbage images into various categories to help users identify and sort waste effectively.

## Dataset

The image classification model is trained using a combination of datasets, as described below:

### Base Dataset: [Garbage Classification](https://www.kaggle.com/datasets/mostafaabla/garbage-classification)
The base dataset, **garbage_classification**, is sourced from Kaggle and contains images of garbage sorted into multiple categories. These categories include 12 classes:
| **Class**      | **Class**       |
|----------------|-----------------|
| battery        | metal           |
| biological     | paper           |
| brown-glass    | plastic         |
| cardboard      | shoes           |
| clothes        | trash           |
| green-glass    | white-glass     |

This dataset serves as the foundation for the classification model.

### Concatenated Dataset: **`garbage_concat`**
The **garbage_concat** dataset is a concatenation of the base dataset and additional images scraped from the internet. This larger dataset aims to enhance the model's performance by providing a broader range of images for training.

### Dataset Preparation
- **Duplicate Cleaning**: All images in the concatenated dataset were carefully inspected and duplicate entries were removed using Python script above.
- **Dataset Split**: The final dataset is split into three sets with the following distribution:
  - **Training Set**: 70% of the total dataset
  - **Validation Set**: 20% of the total dataset
  - **Test Set**: 10% of the total dataset
