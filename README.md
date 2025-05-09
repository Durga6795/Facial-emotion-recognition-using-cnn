# Facial Emotion Recognition using CNN

This project performs **Facial Emotion Recognition (FER)** using a **Convolutional Neural Network (CNN)** trained on the [FER-2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013).

## 📌 Project Overview

We built a deep learning model that can recognize human emotions from grayscale facial images. The model is trained to classify images into 7 emotion categories:

- Angry 😠
- Disgust 🤢
- Fear 😨
- Happy 😄
- Sad 😢
- Surprise 😲
- Neutral 😐

## 🧠 Model Architecture

We used a **classic CNN architecture** with the following components:

- 3 Convolutional layers with ReLU activation
- MaxPooling layers to reduce spatial dimensions
- Dropout for regularization
- Dense layers with softmax output for classification

## 📊 Dataset

- **Dataset**: FER-2013 (Kaggle)
- **Input shape**: 48x48 pixels, grayscale
- **Split**: `train/` and `test/` folders, each with 7 subfolders for each emotion class

## 🔧 Technologies Used

- Python
- TensorFlow / Keras
- Google Colab
- OpenCV (optional for real-time prediction)

## 🏁 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/facial-emotion-recognition-cnn.git
   cd facial-emotion-recognition-cnn
2. Upload the dataset (FER-2013) and unzip it so that it has the following structure:
FER-2013/
  ├── train/
  │    ├── angry/
  │    ├── happy/
  │    └── ...
  └── test/
       ├── sad/
       ├── surprise/
       └── ...
3. Run the notebook in Google Colab or locally.
🚀 Results
Model: Classic CNN (3 conv layers)
Epochs: 50
Test Accuracy: 55.84%
Loss Function: Categorical Crossentropy
Optimizer: Adam
We also experimented with MobileNetV2 (Transfer Learning), but it gave a lower accuracy of 43.62%, likely due to image size and grayscale input incompatibility.

📌 Conclusion
Our CNN model was able to achieve 55.84% accuracy on the FER-2013 dataset. Despite the moderate performance, it effectively captures key facial features for emotion recognition. The challenges faced included low-resolution images, grayscale input, and class imbalance. Further improvements could involve using color datasets, attention mechanisms, and ensemble models.

📷 Sample Predictions (optional)
Add sample images with predicted emotions here if available.

📚 References
FER-2013 Dataset on Kaggle
Keras Documentation




