# **Dog Cat Classification**  

## **Overview**  
This project implements a binary image classification model to distinguish between images of dogs and cats using the MobileNetV2 architecture. The dataset used is the popular Dogs vs. Cats dataset from Kaggle, containing labeled images of dogs and cats.

### **Features**  

- Pretrained MobileNetV2 Model: Leverages transfer learning for faster training and improved performance.
- Transfer Learning: Pretrained weights on ImageNet are used for faster and more efficient training.
- Metrics: Achieves high accuracy and precision across all 10 classes.

Dataset Features:

The Dogs vs. Cats dataset contains 25,000 images of cats and dogs:  

Size:  
Training Set: 20,000 images (10,000 each for dogs and cats).  
Validation/Test Set: 5,000 images.  

# Data Pre-Processing  
- Resized All Images to (224,224)  
- Converted them to RGB  
- Converted them to NumPy Arrays  
- Rescaled all Images  
  
# Model Architecture

base_model = tf.keras.applications.MobileNetV2(input_shape=(224,224,3),include_top=False,weights="imagenet")  
Freeze the base model  
base_model.trainable = False  

model = Sequential([  

  base_model, # if you are using base_model as input layer you dont need to define shape as long as it is defined in the model itself  
  GlobalAveragePooling2D(),  
  Dense(2, activation='sigmoid')  
  
])  

# Model Evaluation:
- Accuracy on Training Data: 99.87%  
- Accuracy on Testing Data: 96.96%  

##### **Getting Started** 
Clone the repo and install dependencies.
