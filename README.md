# 🎥 Sentiment Analysis of Movie Reviews

This project focuses on analyzing movie reviews and classifying them into three categories:  
💚 **Positive** | 🖤 **Neutral** | ❤️ **Negative**  

Since pre-trained models often lack data for neutral sentiment, we developed a custom pipeline using polarity scores for sentiment labeling. Below is an overview of the process:

---

## 🚀 Workflow

### 1️⃣ **Data Integration**  
📂 Reviews were gathered from multiple files (e.g., 2016, 2018, etc.).  
📋 All reviews were combined into a single dataset and saved for further processing.

---

### 2️⃣ **Data Cleaning**  
🧹 The dataset was cleaned to remove unnecessary noise, ensuring high-quality data for analysis.

---

### 3️⃣ **Label Assignment**  
✍️ Since the data lacked predefined labels, we assigned them using **polarity scores**:  
- 💚 **Positive**: Polarity > Threshold  
- ❤️ **Negative**: Polarity < -Threshold  
- 🖤 **Neutral**: Polarity within the threshold range  

---

### 4️⃣ **Handling Class Imbalance**  
⚖️ The dataset was imbalanced, with **positive reviews** dominating while **neutral** and **negative** reviews were sparse.  
To resolve this, we applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance the class distribution, ensuring fairness and avoiding bias in the models.  

---

### 5️⃣ **Model Training**  
📊 Multiple machine learning models were trained to classify the reviews, including:  
- 🤖 **Naive Bayes**  
- 🧠 **Support Vector Machine (SVM)**  
- 🚀 **Gradient Boosting**  
- 🛠️ Other classifiers  

✅ The trained models were saved in `.pkl` format for easy integration with the frontend.

---

## ✨ Features

🎯 **Custom Sentiment Labeling**  
- Reviews are labeled based on polarity scores, enabling neutral sentiment categorization.  

📊 **Balanced Dataset**  
- SMOTE ensures all sentiment classes are equally represented.  

🤝 **Diverse Models**  
- Provides flexibility with multiple pre-trained models to suit different needs.

---

## 🌐 Frontend Integration

The trained models are ready for deployment in a frontend application to provide **real-time sentiment analysis** of user reviews.

---

📢 **Get Started**  
Clone this repository, follow the setup instructions, and start classifying your movie reviews today! 🎉

---

Let me know if you’d like further tweaks or have additional ideas! 😊
