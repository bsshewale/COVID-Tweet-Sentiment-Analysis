

# 🦠 Coronavirus Tweet Sentiment Analysis

### 📊 Project Overview

This project performs **sentiment analysis** on tweets related to the COVID-19 pandemic to understand **public opinion and emotions** during the outbreak. Using **Natural Language Processing (NLP)** and **Machine Learning (ML)** techniques, the model classifies tweets into **Positive**, **Negative**, or **Neutral** sentiments.

---

## 🎯 Objectives

* Analyze public sentiments expressed on Twitter regarding COVID-19.
* Build and evaluate machine learning models for sentiment classification.
* Visualize sentiment distribution to derive actionable insights.

---

## 🧠 Key Features

* Text preprocessing: tokenization, stopword removal, and lemmatization.
* Feature extraction using **CountVectorizer** and **TF-IDF**.
* Implementation and evaluation of multiple ML models.
* Visualization of sentiment distribution and model performance metrics.

---

## 🧰 Tech Stack

**Programming Language:** Python

**Libraries Used:**

* `pandas`, `numpy` – Data handling and preprocessing
* `nltk`, `re`, `string` – Text cleaning and tokenization
* `scikit-learn` – Model building and evaluation
* `matplotlib`, `seaborn`, `wordcloud` – Data visualization
* `joblib` – Model saving and loading

---

## 🗂 Dataset

* Source: [Coronavirus Tweets Dataset](https://github.com/bsshewale/COVID-Tweet-Sentiment-Analysis/blob/main/Coronavirus%20Tweets.csv)
* Contains **40,000+ tweets** labeled as **Positive**, **Negative**, or **Neutral**.

**Key Columns:**

* `OriginalTweet` – The tweet text
* `Sentiment` – The sentiment label (Positive / Negative / Neutral)

---

## ⚙️ Workflow

1. **Data Loading & Cleaning**

   * Removed URLs, mentions, hashtags, and punctuation.
   * Converted all text to lowercase.

2. **Exploratory Data Analysis (EDA)**

   * Visualized most common words.
   * Analyzed sentiment distribution.

3. **Feature Engineering**

   * Used both **CountVectorizer** and **TF-IDF Vectorizer** for text feature extraction.

4. **Model Training & Evaluation**

   * Applied multiple ML algorithms: Logistic Regression, Decision Tree, and KNN.
   * Evaluated models using accuracy, precision, recall, and F1-score.

5. **Visualization**

   * Plotted confusion matrices, sentiment distributions, and word clouds.

---

## 📈 Results

| Model                     | Vectorizer      | Accuracy | F1-Score (Weighted) |
| :------------------------ | :-------------- | :------: | :-----------------: |
| Logistic Regression       | CountVectorizer |  **78%** |       **0.78**      |
| Decision Tree             | CountVectorizer |    70%   |         0.70        |
| K-Nearest Neighbors (KNN) | CountVectorizer |    41%   |         0.41        |
| Logistic Regression       | TF-IDF          |    62%   |         0.62        |
| Decision Tree             | TF-IDF          |    62%   |         0.62        |

✅ **Logistic Regression with CountVectorizer** performed the best overall.

---

## 🧩 Conclusion

In this project, five different **machine learning models** were applied to classify tweet sentiments related to COVID-19. After experimentation with both **CountVectorizer** and **TF-IDF**, the following outcomes were observed:

* **Logistic Regression with CountVectorizer** achieved the **best performance** with **78% accuracy** and a **weighted F1-score of 0.78** — the most efficient and reliable model for this task.
* **Decision Tree with CountVectorizer** showed **moderate performance** (70% accuracy, 0.70 F1-score), being simple and interpretable.
* **K-Nearest Neighbors (KNN)** performed **poorly** with **41% accuracy**, indicating limitations in handling high-dimensional text data.
* **Logistic Regression and Decision Tree with TF-IDF** both achieved **62% accuracy** and **0.62 F1-score**, showing stability but lower efficiency compared to CountVectorizer.

✅ **Final Verdict:**
**Logistic Regression with CountVectorizer** is the **optimal model** for sentiment classification in this dataset, offering a strong trade-off between performance, interpretability, and computational efficiency.

---

## 📊 Visualizations

* Sentiment distribution plots.
* Word clouds for each sentiment category.
* Confusion matrices for model performance.

---

## 🚀 How to Run

1. Clone this repository

   ```bash
   git clone https://github.com/bsshewale/Coronavirus-tweet-sentiment-analysis.git
   cd Coronavirus-tweet-sentiment-analysis
   ```

2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

3. Run the script

   ```bash
   python main.py
   ```

4. View model metrics and visualizations in your console or generated plots.

---

## 💡 Future Enhancements

* Integrate **LSTM** or **BERT** for deep learning-based sentiment analysis.
* Deploy the model using **Streamlit** or **Flask** for interactive usage.
* Enable **real-time sentiment monitoring** via Twitter API integration.

---

## 👨‍💻 Author

**Bharat Shewale**
📧 [bsshewale1630@gmail.com](mailto:bsshewale1630@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/bharatshewale/) | [GitHub](https://github.com/bsshewale)

---

