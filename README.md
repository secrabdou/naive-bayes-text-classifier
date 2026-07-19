# Movie Genre Classifier using Naive Bayes

A machine learning project that classifies movie reviews into their respective genres using Natural Language Processing (NLP) and a Multinomial Naive Bayes model.

## 📊 The Challenge: Class Imbalance & Vocabulary Bias
During development, a fascinating machine learning problem was uncovered:
* **The Imbalance:** The training dataset was heavily skewed, containing **23 Drama reviews** but only **6 Sci-Fi reviews**.
* **The Bias:** Because of this imbalance, the model naturally developed a strong baseline bias toward predicting "Drama." 
* **The Vocabulary Trap:** When tested with a text like *"An incredible alien spaceship engaged in a laser battle..."*, the model still predicted **Drama**. Why? Because words like *spaceship* and *laser* were completely unseen in the small Sci-Fi training set, causing the model to default to its strongest mathematical prior (Drama).
* **The Fix:** The model successfully predicts Sci-Fi only when using the exact vocabulary it learned from during training (e.g., *"mind-bending"* or *"visually ambitious"*), demonstrating how dataset size and feature coverage impact NLP predictions.

## 🛠️ Technologies Used
* **Python**
* **Jupyter Notebook**
* **Scikit-Learn** (CountVectorizer, MultinomialNB)
* **Pandas**

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
