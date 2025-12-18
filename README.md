# ResNet-50 + CBAM (Convolutional Block Attention Module)

![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

This repository contains a Keras implementation of the **ResNet-50** architecture, enhanced with a **Convolutional Block Attention Module (CBAM)** integrated into the final layer. 

## 📖 Overview

While a standard ResNet-50 is a powerful feature extractor, it treats all features equally. By adding **CBAM** (Convolutional Block Attention Module) to the last layer, we allow the model to:
1.  **Focus on Channels (What):** Determine which feature maps are most important for the specific task.
2.  **Focus on Space (Where):** Determine which parts of the image contain the most relevant information.

This implementation uses the **ImageNet pre-trained weights** for the ResNet backbone and appends the attention mechanism before the classification head.

---

## 🧠 Architecture Details

### 1. ResNet-50 Backbone
The model uses the standard ResNet-50 architecture. The attention block is inserted right after the last convolutional output but before the Global Average Pooling layer.

### 2. CBAM Module
The module consists of two sequential sub-modules:
*   **Channel Attention:** Exploits the inter-channel relationship of features.
*   **Spatial Attention:** Exploits the inter-spatial relationship of features.

---
## 📝 Citation

If you use this implementation in your research or project, please cite it using the following formats:

### BibTeX
```bibtex
@misc{resnet50_cbam_keras,
  author = {Your Name},
  title = {ResNet-50 Enhanced by CBAM Implementation in Keras},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/your-username/your-repo-name}}
}
