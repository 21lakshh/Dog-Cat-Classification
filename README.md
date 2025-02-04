# 🐶🐱 Dog-Cat Classification using MobileNetV2

This repository contains a deep learning project that classifies images of dogs and cats. The model leverages **transfer learning** using the **MobileNetV2** architecture pretrained on ImageNet. The project achieves **99.87% training accuracy** and **96.96% test accuracy**.

---

## 🚀 Features

- **Transfer Learning**: Utilized MobileNetV2 for high performance on image classification tasks.
- **Image Preprocessing**: Input images were rescaled by dividing pixel values by 255.
- **High Accuracy**: Achieved impressive accuracy on both training and test datasets.
- **Scalable Architecture**: Suitable for use in real-world scenarios with minimal fine-tuning.

---

## 💂️ Dataset

- The dataset consists of labeled images of dogs and cats.
- Images were preprocessed as follows:
  - Rescaled pixel values by dividing by **255** for normalization.

---

## 📊 Model Performance

| **Metric**        | **Accuracy** |
|--------------------|--------------|
| Training Accuracy  | 99.87%       |
| Test Accuracy      | 96.96%       |

---

## 🛠️ Technology Stack

- **Programming Language**: Python
- **Deep Learning Framework**: TensorFlow/Keras
- **Pretrained Model**: MobileNetV2 (Transfer Learning)

---

## 📖 How It Works

1. **Data Pre-Processing** 
    - Resized All Images to (224,224)  
    - Converted them to RGB  
    - Converted them to NumPy Arrays  
    - Rescaled all Images 

2. **Model Architecture**:
   - Base model: MobileNetV2 pretrained on ImageNet.
   - Custom fully connected layers added for binary classification (dog vs. cat).

3. **Training**:
   - The model was fine-tuned on the dog-cat dataset.
   - Early stopping was used to prevent overfitting.

4. **Evaluation**:
   - The model was evaluated on a separate test set, achieving high accuracy.
  
---

## 🎯 Results

The model performs well on unseen data, demonstrating its ability to generalize.

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for any enhancements or bug fixes.

---

## 🌟 Acknowledgments

- **MobileNetV2**: For providing an excellent base model for transfer learning.
- The open-source community for inspiration and resources.
