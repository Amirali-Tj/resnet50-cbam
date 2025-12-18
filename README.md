# ResNet-50 + CBAM Implementation (Keras)

![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)

This project implements a **ResNet-50** architecture enhanced with a **Convolutional Block Attention Module (CBAM)** in the final layer using Keras/TensorFlow.

## 📖 Introduction
Standard ResNet-50 models are excellent at feature extraction. However, by adding **CBAM**, we allow the model to perform "Adaptive Feature Refinement." 

The model focuses on:
1. **Channel Attention:** Which features (channels) are important?
2. **Spatial Attention:** Where in the image are those features located?

## 🛠️ Installation

```bash
git clone https://github.com/your-username/your-repo-name.git
pip install tensorflow numpy
