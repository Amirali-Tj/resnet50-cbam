ResNet-50 + CBAM Implementation in Keras
![alt text](https://img.shields.io/badge/Framework-Keras%20/%20TensorFlow-orange)

![alt text](https://img.shields.io/badge/License-MIT-blue.svg)
This repository provides an implementation of a ResNet-50 architecture enhanced with the Convolutional Block Attention Module (CBAM). By integrating CBAM into the final layer of the ResNet-50 backbone, the model learns to focus on "what" (channel attention) and "where" (spatial attention) the most important features are before making a classification.
🚀 Overview
Standard ResNet-50 is powerful but treats all spatial regions and channels with equal importance. CBAM (Convolutional Block Attention Module) is a simple yet effective attention module for feed-forward convolutional neural networks.
Why CBAM?
Channel Attention: Focuses on the "what" by identifying which feature maps (channels) are most meaningful.
Spatial Attention: Focuses on the "where" by identifying which parts of the image are most informative.
Performance: Significant boost in accuracy with negligible increase in computational overhead.
🏗️ Model Architecture
The model follows this workflow:
Backbone: Pre-trained ResNet-50 (ImageNet weights) up to the last convolutional layer.
Attention: The output of ResNet-50 is passed through the CBAM block.
Global Average Pooling: Reducing spatial dimensions.
Output: Fully connected layer for the specific classification task.
