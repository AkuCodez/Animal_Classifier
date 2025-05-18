# 🐾 Animal Image Classifier

## 🔍 Objective
A deep learning model built to classify animal images into 15 categories using transfer learning (MobileNetV2). Trained on a dataset of labeled animal photos, each resized to 224x224 pixels.

## 📁 Dataset
The dataset consists of 15 animal classes:
- Bear, Bird, Cat, Cow, Deer, Dog, Dolphin, Elephant, Giraffe, Horse, Kangaroo, Lion, Panda, Tiger, Zebra

## 🧠 Model Summary
- **Base Model**: MobileNetV2 (pretrained on ImageNet)
- **Layers Added**: GlobalAveragePooling2D → Dense (ReLU) → Dense (Softmax)
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Augmentation**: Rotation, Shear, Zoom, Shift, Flip

## 📈 Results
- **Training Accuracy**: ~95%
- **Validation Accuracy**: ~90% (may vary)
- **Evaluation**: Prediction tested on multiple unseen images

## 🖼️ Example Predictions

See folder: `/example_predictions`

Each image is labeled with its predicted class and confidence score.

Example:
![Example Prediction](example_predictions/predicted_elephant.jpg)

## 🚀 How to Run the Project

1. Open `model_training.ipynb` in [Google Colab](https://colab.research.google.com).
2. Mount your Google Drive if using a dataset stored there.
3. Train the model or load the pretrained `best_model.h5`.
4. Upload new images and run the prediction code to classify them.

## 📦 Files in the Project
- `model_training.ipynb` — Model training and prediction notebook
- `best_model.h5` — Trained Keras model (optional)
- `example_predictions/` — Test images and prediction results
- `README.md` — Project documentation

## 🛠 Tools Used
- TensorFlow / Keras
- MobileNetV2 (Transfer Learning)
- Google Colab
- Python (matplotlib, numpy, os)

---

## 📌 Credits
Project by Akshaj Tiwari as part of an Image Classification assignment.

