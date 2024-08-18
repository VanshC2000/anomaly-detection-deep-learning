# Detecting anomalies in standardised goods using deep learning

## Objective
This project explores the use of deep learning to automate the inspection process of finished, standardised goods using deep learning models. This is to reduce the significant costs incurred in manually inspecting goods at the end of the production process. Such a system would also reduce the cost of quality (CoQ) for an organisation, which is defined as an estimated measure of the cost an organization faces due to the production of goods that are below the required quality. The American Society for Quality estimates that costs of poor quality in an established organisation are as much as 10-15% of operations.

## Dataset
For this study, an anomaly detection dataset compiled by MVTec was used (Bergmann, Batzner, Fauser et al, 2021). This dataset was compiled for the purpose of testing different anomaly detection methods with a focus on the inspection of standardised, industrial goods. MVTec has distinct datasets for different industrial products, and the dataset containing optical fibre cable images was used for the purpose of this study. 

In the dataset, there were 224 images of ‘normal’ optical fibre cables, and 92 images of cables that had visible anomalies. It can be downloaded [here](https://www.mvtec.com/company/research/datasets/mvtec-ad).

## Models used
- Simple neural network: There were 2 dense layers in this model with a ReLU activation function
- Convolutional neural network
- VGG16: This is a convolutional neural network (CNN) architecture renowned for its simplicity and depth.
- ResNet 50: This is a model widely used in various computer vision applications, including object detection, image classification, and more, due to its ability to learn rich and complex feature representations.

## Results
To identify anomalies in a dataset of finished product images, developing a convolutional neural network based on VGG16 yielded the best results. Following were the results from the test data:
- Loss: 0.506
- Accuracy: 0.816
- Recall: 1.000
- F2 score: 0.953
