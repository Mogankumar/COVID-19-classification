# Deep Learning Project: COVID-19 Classification from Chest X-Rays

This project focuses on developing a two-layer deep learning model for automated classification of chest X-ray images into three categories: Normal, COVID-19, and Viral Pneumonia. By leveraging a two-step classification approach and convolutional neural networks (CNNs), the model achieves high accuracy in diagnosing COVID-19, aiding in early detection and intervention.

**Project Overview**

Problem Statement

The goal of the project is to build a deep learning model capable of:
	1.	Classifying images as Normal or Abnormal.
	2.	Further classifying abnormal images into COVID-19 or Viral Pneumonia.

Approach

The solution consists of two classifiers:
	•	Classifier 1: Identifies whether an image is “Normal” or “Abnormal”.
	•	Classifier 2: Further classifies “Abnormal” images into “COVID-19” or “Viral Pneumonia”.

 Dataset
	•	Classes: Normal, COVID-19, Viral Pneumonia
	•	Dataset consists of grayscale X-ray images with varying levels of abnormality.
	•	Data preprocessing includes normalization and resizing to fit the CNN input.

 Proposed Architecture

Both classifiers use a similar CNN architecture:
1.	Convolutional Layer:
  	•	32 filters of size 3 * 3.
  	•	Activation: ReLU
2.	Pooling Layer:
	  •	Max-pooling with a pool size of 2 * 2.
3.	Flattening Layer:
  	•	Converts 2D feature maps into a 1D array.
4.	Dropout:
	  •	Dropout rate of 0.3 to prevent overfitting.
5.	Dense Layers:
	  •	Fully connected layer with 32 units (ReLU activation).
	  •	Output layer with 1 unit (Sigmoid activation for binary classification).

Conclusion
1. The two-layer CNN architecture effectively classifies chest X-ray images into Normal, COVID-19, and Viral Pneumonia with high accuracy.
2. Classifier 1 Accuracy: ~91%
3. Classifier 2 Accuracy: ~96%
4. The model demonstrates the potential for deep learning to assist in early diagnosis and treatment of COVID-19.


   
