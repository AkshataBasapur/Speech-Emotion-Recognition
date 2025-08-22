🎙️ Speech Emotion Recognition with Autoencoders

This project implements a deep learning pipeline for Speech Emotion Recognition (SER) and Emotion Intensity Estimation using autoencoder-based latent audio features. The system leverages MFCCs for feature extraction and employs a multi-task learning framework to perform both emotion classification and intensity prediction simultaneously.

🚀 Features
Extracts Mel-Frequency Cepstral Coefficients (MFCCs) from speech.
Uses a fully connected autoencoder for feature compression.
Dual-branch network:
Classification Module → Predicts categorical emotions (8 classes).
Regression Module → Estimates emotional intensity on a continuous scale.
Multi-task learning for better generalization.
Achieves:
92.36% classification accuracy
0.1523 Mean Absolute Error (MAE) for intensity prediction.

📂 Dataset
RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
1,440 audio samples across 8 emotions:
Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised
Each emotion expressed at 2 intensity levels (normal & high).

🛠️ Methodology
Preprocessing: Convert raw audio → MFCC features (using Librosa).
Autoencoder: Learn compact latent features from MFCCs.
Classification Head: Softmax layer for 8-class emotion recognition.
Regression Head: MLP/LSTM for intensity prediction.
Multi-task Training: Joint optimization of classification (cross-entropy) & regression (MSE) losses.

📊 Results
Metric	Value
Accuracy	92.36%
MAE	0.1523
MSE	0.0380

Emotion-wise F1-Scores:
Angry: 0.95 | Disgust: 0.96 | Fearful: 0.96
Happy: 0.93 | Neutral: 0.93 | Sad: 0.88
Calm: 0.90 | Surprised: 0.89

📌 Applications

Emotionally aware chatbots & voice assistants
Mental health monitoring tools
Customer service analytics
Education & e-learning systems
