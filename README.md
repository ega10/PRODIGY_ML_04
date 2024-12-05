# PRODIGY_ML_04
Hand Gesture Recognition using Convolutional Neural Network
This project involves developing a hand gesture recognition system using a Convolutional Neural Network (CNN). The model is trained to classify 10 different hand gestures based on grayscale images. This project aims to enable intuitive human-computer interaction using hand gestures.

Dataset
The dataset used contains images of hand gestures categorized into 10 classes:

Palm
L
Fist
Fist Moved
Thumb
Index
OK
Palm Moved
C
Down
Dataset Structure
The dataset consists of two directories: train and test.
Each directory contains subfolders named after gesture categories (e.g., 01_palm, 02_l, etc.).
Images are in grayscale format.
Model Architecture
The model uses a CNN to classify gestures. Below are the architectural details:

Layers
Convolutional Layers: Extract spatial features from images.
3 convolutional layers with increasing filters (32, 64).
MaxPooling Layers: Downsample feature maps.
Dropout Layers: Prevent overfitting by dropping out neurons during training.
Dense Layers: Fully connected layers for classification.
A final dense layer with a softmax activation for multi-class classification.
Model Summary
Input Shape: (50, 50, 1) (grayscale images resized to 50x50 pixels)
Total Parameters: 1,669,290
Optimizer: RMSProp
Loss Function: Categorical Crossentropy
Metrics: Accuracy
Training Process
Data Preprocessing:

Images resized to 50x50 pixels.
Pixel values normalized to the range [0, 1].
Labels converted to one-hot encoding.
Data split into training (70%) and testing (30%).
Training Details:

Epochs: 7
Batch Size: 32
Validation on test set.
Results:

Training Accuracy: ~99.98%
Validation Accuracy: ~99.97%
Evaluation
Performance Metrics
Test Accuracy: 99.97%
Confusion Matrix: Visualized to observe classification performance across all classes.
Visualizations
Model Loss and Accuracy:

Loss and accuracy plotted for both training and validation datasets over epochs.
Confusion Matrix:

Heatmap generated to show the prediction accuracy of each class.
