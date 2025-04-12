
# 🧠 Facial Emotion Recognition with CNN-LSTM  
🚀 Trained on FER-2013 Dataset | 🏆 Accuracy Achieved: **84%**

---

## 📌 Project Summary

**Facial Emotion Recognition (FER)** is a powerful tool in computer vision that helps machines understand human emotions through facial expressions.  

In this project, we propose a hybrid **CNN-LSTM** architecture that excels at recognizing **7 core emotions** from grayscale face images.

- 💡 **Model Accuracy:** 84% using the **FER-2013** dataset  
- 🤖 **Architecture:** CNN for spatial features + LSTM for temporal representation  
- 📊 **Output:** Emotion classification + Performance visualization

---

## 🗂️ Dataset: FER-2013

| Property    | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| 📁 Dataset   | [FER-2013 on Kaggle](https://www.kaggle.com/datasets/msambare/fer2013)     |
| 🖼️ Images    | 48x48 pixels, grayscale                                                    |
| 😊 Emotions  | Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral                        |
| 🔢 Samples   | 35,887 (Training: 28,709, Testing: 7,178)                                   |

---

## 🏗️ Model Architecture

Input Image (48x48x1) ↓ Convolutional Layers ↓ MaxPooling Layers ↓ Flatten Layer ↓ LSTM Layer ↓ Fully Connected Layers ↓ Softmax Output (7 classes)

yaml
Copy
Edit

### 📌 Why CNN-LSTM?

- 🧠 **CNN** captures spatial features from facial structures  
- 🔄 **LSTM** models sequential dependencies in flattened pixel arrays  
- 🔬 Together, they form a robust system for emotion recognition

---

## 🏁 Training Details

| Setting         | Value                    |
|------------------|--------------------------|
| ⚙️ Optimizer      | Adam                     |
| 🔧 Loss Function | Categorical Crossentropy |
| 🔁 Epochs        | 50                       |
| 📦 Batch Size    | 64                       |
| 🧪 Augmentation  | Rotation, Zoom, Flip     |

---

## 📈 Performance & Results

✅ **Achieved Accuracy:** **84%** on the private test set  

📊 Visual outputs include:

- 📉 **Confusion Matrix**  
  ![Confusion Matrix](https://github.com/user-attachments/assets/c48a9548-a3d4-4efc-a527-47ffcdac1490)

- 📈 **Training/Validation Accuracy & Loss Curves**  
  ![Training Curve 1](https://github.com/user-attachments/assets/33a16d48-e8d9-42be-bb12-52c04803a7b4)  
  ![Training Curve 2](https://github.com/user-attachments/assets/d3756927-b7b1-495f-aeee-1d2b8ae6d390)

- 🔍 **Sample Predictions with Emotion Labels**  
  ![Prediction Example](https://github.com/user-attachments/assets/8ba777fb-2689-44a2-a5cc-c19a621e1d3d)

---
## 🧪 Run Inference

```python
# Example: Predict emotion from an image
emotion = predict_emotion('your_image.png')
print("Predicted Emotion:", emotion)
```
🎯 The model returns one of the following emotions:

['Angry', 'Disgust', 'Fear', 'Happy', 'Sad', 'Surprise', 'Neutral']

---
## 📜 License
This repository is the original work of Md. Akash Hosen.
It is protected by a custom license – please do not reuse, redistribute, or modify without prior permission.

👉 Want to use this project? Kindly contact the author first.
---
👨‍💻 Author
Md. Akash Hosen
🎓 Computer Science and Engineering | 💡 Deep Learning Enthusiast
🌐 GitHub   |   ✉️ akashcse20@gmail.com


