# Concrete-Crack-Image-Detection

# 🧱 Surface Crack Detection – Deep Learning Project (CNN)
## 📌 Overview
- This project focuses on automated detection of concrete surface cracks using a Convolutional Neural Network (CNN). The model is trained on a high-quality dataset of concrete images from Kaggle and achieves 97.56% test accuracy.
- This system can assist engineers, inspectors, and construction teams in detecting cracks early — improving safety, reducing maintenance costs, and enabling real-time monitoring.

🎯 Problem Statement
Concrete structures naturally degrade over time. Manual inspection is:
* Time-consuming
* Error-prone
* Expensive
* Not scalable for large infrastructure
The goal of this project is to:
* Build a CNN model that can automatically classify images as Crack or Non-Crack
* Achieve high accuracy suitable for real-world use
* Provide a reusable pipeline for preprocessing, training, evaluation, and prediction
* Enable future deployment in mobile apps, IoT devices, or inspection robots

🧾 Dataset Information
Dataset Source: Kaggle Dataset Name: Surface Crack Detection 🔗 https://www.kaggle.com/datasets/arunrk7/surface-crack-detection/data
📅 Dataset Details
* Total Images: 40,000
* Crack Images (Positive): 20,000
* Non-Crack Images (Negative): 20,000
* Format: .jpg
* Resolution: 227×227 pixels
* Balanced classes: Yes
📂 Required Folder Structure
After downloading the dataset, place it in the following format:

data/
 ├── Positive/
 └── Negative/

🧠 Model Approach
A custom Convolutional Neural Network (CNN) was built using TensorFlow/Keras. The model includes:
* Multiple Conv2D layers
* MaxPooling for spatial reduction
* Dropout for regularization
* Dense layers for classification
* Softmax output layer
The full architecture is available inside the notebook:
📄 Crack Image Detection.ipynb

📊 Model Performance
✔ Classification Report
Class	Precision	Recall	F1-Score	Support
NEGATIVE	0.96	0.99	0.98	917
POSITIVE	0.99	0.96	0.97	883
Overall Accuracy	97.56%			1800
✔ Final Test Metrics
* Test Loss: 0.09563
* Test Accuracy: 97.56%
The model successfully generalizes well with strong performance across both classes.

📊 Metrics Tracked
This project evaluates several key metrics:
* Accuracy
* Precision
* Recall
* F1-score
* Loss curves
* Confusion matrix (optional to add)
These metrics help validate the model’s reliability for real-world use.

🖼 Example Predictions
The notebook includes predictions such as:
* Crack Detected ✔️
* No Crack Detected ❌
You can add your own sample images to a folder like:

samples/
 ├── crack1.jpg
 └── nocrack1.jpg
And display predictions using the notebook.
