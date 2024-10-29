<h1>Action Recognition with Convolutional LSTM on UCF50</h1>

<p>This repository contains an action recognition model built using Convolutional LSTM, specifically designed for video classification on the UCF50 dataset. The model combines 3D Convolutional Neural Networks (3D CNN) with LSTMs to capture spatial and temporal features effectively. The model achieves over 80% validation accuracy on the dataset.</p>

<h2>Model Architecture</h2>

<p>The architecture leverages multiple 3D convolutional layers for spatial feature extraction, followed by max-pooling and dropout layers to reduce overfitting. The feature maps are flattened and fed through fully connected layers for final classification.</p>

<h3>Summary of Layers:</h3>
<ul>
    <li><strong>Conv3D Layers</strong>: Extracts spatial features across video frames with increasing depth.</li>
    <li><strong>MaxPooling3D Layers</strong>: Reduces spatial dimensions while retaining critical features.</li>
    <li><strong>Dropout Layers</strong>: Applied after pooling to prevent overfitting.</li>
    <li><strong>Flatten Layer</strong>: Transforms 3D outputs to 1D for dense layer input.</li>
    <li><strong>Dense Layers</strong>: Final fully connected layers to classify actions.</li>
</ul>
