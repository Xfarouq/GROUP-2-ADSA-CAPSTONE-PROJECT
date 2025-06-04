# Malaria Detection Using Deep Learning

This repository contains the code for the Arewa Data Science Capstone Project by Group 2, focused on automating malaria diagnosis using deep learning. The project leverages the ResNet18 architecture in PyTorch to classify red blood cell images as either parasitized or uninfected. The primary goal is to support faster and more accurate diagnosis of malaria in resource-limited settings.

## Project Overview

Malaria remains a significant public health challenge in many tropical regions, particularly in sub-Saharan Africa. Traditional diagnostic methods, while effective, are often time-consuming and require trained professionals. This project aims to bridge that gap by developing an AI-powered solution that can automatically detect malaria from microscopic blood smear images using deep learning models.

## Team Members

* Umar Lawan Sani
* Yusuf Aliyu
* Surajo Nuhu Umar
* Amalai Rham Machunga

## Dataset

The dataset used for this project is the publicly available “Cell Images for Malaria” dataset, containing 27,558 images evenly divided into two classes: parasitized and uninfected red blood cells. The dataset was split into training, validation, and test sets (e.g., 70%-20%-10%) and preprocessed with resizing and normalization to improve model performance.

## Methodology

We implemented the ResNet18 model using PyTorch. The network was initialized with ImageNet pre-trained weights and fine-tuned for binary classification. Key steps include:

* Freezing the initial convolutional layers for feature extraction
* Replacing the final fully connected layer with a custom classifier
* Using Binary Cross Entropy loss
* Optimizing with the Adam optimizer (learning rate = 0.0001)

## Results

The model achieved a test accuracy of approximately 93%, with strong precision and recall metrics. Training and validation performance were visualized using matplotlib to track convergence and avoid overfitting.

## Deployment

The trained model is deployed via a Gradio web application that allows users to upload blood smear images and get instant predictions on whether the cell is infected with malaria or not.

👉 Demo Link: https://drive.google.com/file/d/1JLiv7s4NYEIqIHU7Owsbgp-1QCJJBVZz/view?usp=drivesdk

## Future Work

* Improve model accuracy by experimenting with deeper networks (e.g., ResNet50 or EfficientNet)
* Integrate multi-class classification to identify different Plasmodium species
* Develop a mobile app version for on-the-ground testing in rural clinics

## Contributions

We welcome community contributions to expand the dataset, improve classification performance, or enhance the Gradio app’s usability.

## Acknowledgments

Special thanks to the Arewa Data Science Academy, our mentors ***Engr. Mustapha Abdullahi*** and ***Dr. Sani Aji*** for their unwavering support. Gratitude also goes to our peers and facilitators for their valuable input throughout the project.
