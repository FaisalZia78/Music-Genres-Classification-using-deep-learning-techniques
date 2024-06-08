# Music-Genres-Classification
Introduction
The goal of this project is to classify music tracks into predefined genres using an Inception V3 model. Inception V3 is a widely used CNN architecture, originally developed for image classification but adapted here for audio classification by converting audio signals into spectrograms.

Dataset
The dataset used for this project should be a collection of audio files labeled by genre. Here’s how to prepare the dataset:
we have used GTZAN dataset for this project.
Audio Files: Collect audio files categorized into different genres.

Preprocessing:
Convert audio files into spectrograms or mel-spectrograms.
Normalize and resize the spectrogram images to fit the input dimensions required by Inception V3.
This project uses the Inception V3 architecture, modified for spectrogram image input:

Base Model: Pre-trained Inception V3 (excluding the top layers).
New Layers: A global average pooling layer followed by fully connected dense layers and a softmax layer for classification.
Transfer Learning: The pre-trained weights of Inception V3 are used to benefit from its ability to extract features, and additional layers are trained on the spectrogram images of music genres

Results
The results of the model training and evaluation include:

Accuracy: The overall accuracy of the model on the test dataset.
Confusion Matrix: A confusion matrix to visualize performance across different genres.
Classification Report: Precision, recall, and F1-score for each genre.
