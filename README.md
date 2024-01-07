# Melanoma Detection Case Study
---
## Case study assignment by IIIT Bangalore and Upgrad
---
> - Solving this assignment will give an idea of analysing the dataset and build a CNN model to classify the image into one of the nine disease category.
> - Developed as part of the Deep Learning Module required for Executive Post Graduate Program in Machine Learning and AI - IIIT,Bangalore.
---

## Table of Contents
* [General Information](#general-information)
* [Methodology](#methodology)
* [Repository contents](#repository-contents)
* [Conclusion](#conclusion)

## General Information
**Objective:**
- Build a **CNN based model** which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths.
- A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

**Dataset:**

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Methodology
- Data Reading/Data Understanding
- Dataset Creation
- Dataset visualisation
- Model Building & training
- Data Augmentation
    - Model Building & training on the augmented data
- Class distribution
    - Handling class imbalances
    - Model Building & training on the rectified class imbalance data
- Analysis on unseen test data

## Repository contents
| File | Description |
|:-----|:------------|
| Python notebook | It contains the complete detailed code along with necessary output to solve the problem. |
| README.md | This file briefs about the project. |
| Skin cancer ISIC The International Skin Imaging Collaboration\Train\ | Contains the train dataset. |
| Skin cancer ISIC The International Skin Imaging Collaboration\Train\\*\\output | Contains the augmented train dataset. |
| Skin cancer ISIC The International Skin Imaging Collaboration\Test\ | Contains the test dataset. |

## Conclusion
The solution has 9 models, and the below report shows the train, validation and test accuracy obtained using each model.

|index|Model|Train Accuracy|Validation Accuracy|Test Accuracy|
|---|---|---|---|---|
|8|Base model + Augmentation Layer + more dropout layers + more batch norm layer \(Modification\) with Class balance|0\.74|0\.67|0\.53|
|5|Base model + Augmentation Layer + more dropout layers + 1 batch norm layer with Class balance|0\.68|0\.57|0\.45|
|2|Base Model + Augmentation Layer + 1 dropout layer|0\.6|0\.55|0\.42|
|4|Base Model + Augmentation Layer + more dropout layers with Class balance|0\.59|0\.59|0\.42|
|6|Base model + Augmentation Layer + more dropout layers + more batch norm layer with Class balance|0\.72|0\.45|0\.39|
|1|Base Model + Augmentation Layer|0\.59|0\.56|0\.38|
|3|Base Model + Augmentation Layer + more dropout layers|0\.55|0\.49|0\.32|
|7|Base model + Augmentation Layer + more dropout layers + more batch norm layer \(reposition\) with Class balance|0\.77|0\.45|0\.3|
|0|Base Model|0\.93|0\.55|0\.29|

- From the above report, we could see that the class balance and augmentation strategy works well.
- The best metrics got from this experiment is *Train accuracy* of **0.74**, *Validation Accuracy* of **0.67** and *Test Accuracy* of **0.53**.

## Contact
Created by [@shruthipv96] - feel free to contact me!
