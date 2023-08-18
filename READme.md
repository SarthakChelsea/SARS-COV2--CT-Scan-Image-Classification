# SARS Cov-2 CT Scan Image Classification Project

![Project Banner](https://www.mdpi.com/diagnostics/diagnostics-11-00893/article_deploy/html/images/diagnostics-11-00893-g002.png) 

This repository contains the code and resources for the **Brain CT Scan Image Classification** project. The project focuses on using transfer learning to classify brain CT scan images into different categories and deploying the trained model using Flask.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Transfer Learning](#transfer-learning)
- [Model Deployment](#model-deployment)
- [Setup](#setup)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Medical image classification plays a crucial role in assisting healthcare professionals to accurately diagnose various medical conditions. This project aims to utilize transfer learning, a technique where a pre-trained model is fine-tuned on a new dataset, to classify brain CT scan images into different categories such as normal or Covid

## Dataset

The dataset for this project comprises a collection of brain CT scan images sourced from SARS-COV-2 Ct-Scan Dataset in kaggle. It includes labeled images belonging to 2 classes, namely as nonCovid and Covid. The dataset is preprocessed and split into training, validation, and testing sets.

## Transfer Learning

Transfer learning is employed to leverage the knowledge learned by a pre-trained neural network on a large dataset to improve the performance of our model on a smaller dataset. We use the VGG16 as a base model and fine-tune its layers to adapt it to our specific classification task.

## Model Deployment

The trained model is deployed using Flask, a web framework for Python. The deployment allows users to upload a brain CT scan image through a web interface, and the model predicts the class of the uploaded image. The prediction result is then displayed on the web page.

![Deployment Model](https://drive.google.com/file/d/1tvIedqQMsd4ZJHpEfwTWO9aFgQ8n6_Nl/view?usp=sharing) 

## Setup

To contribute to the project or modify the code, follow these steps:

1. Fork the repository to your GitHub account.
2. Clone the forked repository to your local machine.
3. Create a new branch for your changes
4. Make your modifications and additions to the code.
5. Commit and push your changes to your GitHub repository.
6. Create a pull request from your branch to the original repository's `main` branch.



---

**Disclaimer:** This project is for educational purposes and should not be used in real-world medical diagnoses without proper validation and professional oversight.

For questions or inquiries, please contact sarthakchelsea@gmail.com.

[Optional: Add acknowledgments, references, or additional sections as needed.]

 Data Source: www.kaggle.com/plameneduardo/sarscov2-ctscan-dataset
 VGG16 documentation: https://conx.readthedocs.io/en/latest/VGG16%20and%20ImageNet.html
