# Action Recognition with Convolutional LSTM on UCF50
This repository contains an action recognition model built using Convolutional LSTM, specifically designed for video classification on the UCF50 dataset. The model combines 3D Convolutional Neural Networks (3D CNN) with LSTMs to capture spatial and temporal features effectively. The model achieves over 80% validation accuracy on the dataset.

Model Architecture
The architecture leverages multiple 3D convolutional layers for spatial feature extraction, followed by max-pooling and dropout layers to reduce overfitting. The feature maps are flattened and fed through fully connected layers for final classification.

Summary of Layers:
Conv3D Layers: Extracts spatial features across video frames with increasing depth.
MaxPooling3D Layers: Reduces spatial dimensions while retaining critical features.
Dropout Layers: Applied after pooling to prevent overfitting.
Flatten Layer: Transforms 3D outputs to 1D for dense layer input.
Dense Layers: Final fully connected layers to classify actions.
