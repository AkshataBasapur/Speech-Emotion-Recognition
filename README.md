# 🎙️ Speech Emotion Recognition with Autoencoders

This project focuses on **Speech Emotion Recognition (SER)** and **Emotion Intensity Estimation** using a **deep learning pipeline**. The system extracts **MFCC features** from speech, compresses them using an **autoencoder**, and applies a **multi-task learning framework** with two branches:  
- **Emotion Classification** (8 categories)  
- **Intensity Prediction** (continuous scale)  

---

## 📂 Dataset
- **Source**: RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)  
- **Samples**: 1,440 audio recordings  
- **Emotions**: Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised  
- **Intensity**: Normal & High  

---

## 🤖 Algorithms / Models Used
- Autoencoder (feature compression)  
- Classification Head (Softmax for categorical prediction)  
- Regression Head (MLP/LSTM for intensity prediction)  
- Multi-task learning framework  

---

## 📊 Evaluation Metrics
- **Accuracy**  
- **Mean Absolute Error (MAE)**  
- **Mean Squared Error (MSE)**  
- **F1-Score (per emotion)**  

---

## 🏆 Key Results
- **92.36% classification accuracy**  
- **MAE: 0.1523** for intensity prediction  
- High F1-scores for most emotions (≥0.90)  

---

## 📌 Applications
- Emotionally aware **chatbots & voice assistants**  
- **Mental health monitoring** tools  
- **Customer service analytics**  
- **Education & e-learning systems**  

---
