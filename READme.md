# SARS-CoV-2 CT Scan Image Classification Project
![Project Banner](https://media.springernature.com/lw685/springer-static/image/art%3A10.1007%2Fs10489-020-01831-z/MediaObjects/10489_2020_1831_Fig6_HTML.png) 

This repository contains code and resources for a project focused on classifying SARS-CoV-2 CT scan images using transfer learning with the VGG16 model. The project also includes the deployment of the trained model using Flask to classify whether a patient has COVID-19 or not based on CT scans. The achieved accuracy on the test set is 88%.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Usage](#usage)
- [Installation](#installation)
- [Deployment](#deployment)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

The outbreak of the SARS-CoV-2 virus has led to a global pandemic. CT scan images have proven to be useful in diagnosing COVID-19 cases. This project aims to build a classification model using transfer learning with the VGG16 architecture to automatically identify whether a patient has COVID-19 based on their CT scan images. The model is then deployed using Flask for easy and user-friendly access.

## Dataset

The dataset used for this project contains a collection of CT scan images from patients, some of whom have been diagnosed with COVID-19 and others who have not. The dataset was  taken by Kaggle. It has 2 folders, one with CT scans of non-covid patients and one with CT scans of covid patients.

## Methodology

1. **Data Preprocessing**: The CT scan images were preprocessed by resizing and normalizing them to ensure they can be fed into the VGG16 model.

2. **Transfer Learning with VGG16**: The VGG16 model pre-trained on ImageNet was used as the base model. The final classification layer was replaced with a new layer for categorical classification (COVID-19 vs. Non-COVID-19).

3. **Model Training**: The modified VGG16 model was trained on the dataset using appropriate training parameters. Al parameters were untrained so that they could be trained on our training set

4. **Model Evaluation**: The trained model was evaluated on a test set to measure its performance, resulting in an accuracy of 88%.

## Results

The final model achieved an accuracy of 88% on the test set, demonstrating its effectiveness in classifying CT scan images for COVID-19 diagnosis.

## Usage

To use the code in this repository:

1. Clone the repository: `git clone https:/SarthakChelsea/github.com//SARS-COV2--CT-Scan-Image-Classification.git`
2. Navigate to the project directory: `cd sars-cov-2-ct-classification`
3. Follow the installation instructions to set up the required dependencies.
4. Run the classification script to see how the model performs on sample CT scan images.
5. Follow the deployment instructions to deploy the model using Flask.


## Deployment

The model can be deployed using Flask to create a web application for users to upload CT scan images and receive predictions. The deployment involves:

1. Creating a Flask web application.
2. Loading the trained model.
3. Creating an HTML form for file upload.
4. Processing the uploaded image and making predictions.
5. Displaying the prediction results.

## Conclusion

This project demonstrates the successful application of transfer learning with the VGG16 model to classify SARS-CoV-2 CT scan images. The deployment of the model using Flask allows for real-world usage and easy access to the classification service.

## References

Data Source: https://www.kaggle.com/datasets/plameneduardo/sarscov2-ctscan-dataset

VGG16 documentation: https://conx.readthedocs.io/en/latest/VGG16%20and%20ImageNet.html

Feel free to customize this Markdown file to suit your project structure and content.
