# 💬 Intern Feedback Sentiment Analysis

A Machine Learning project that analyzes intern feedback and reviews
to classify sentiments as Positive, Negative, or Neutral — helping
organizations identify areas where intern satisfaction can be improved.

---

## 📌 Objective

Analyze intern feedback to understand positive and negative sentiments
and identify areas where intern satisfaction can be improved.

---

## 📊 Dataset

| Column | Description |
|---|---|
| intern_id | Unique intern identifier |
| feedback_text | Actual written feedback from intern |
| sentiment | Positive / Negative / Neutral (target) |
| rating | Star rating 1 to 5 |
| department | Engineering, HR, Finance, Marketing etc. |
| mentor_available | Yes / No / Sometimes |
| work_life_balance | Score 1 to 5 |
| learning_score | Score 1 to 5 |
| would_recommend | 1 = Yes, 0 = No |

- Total Records: 300
- Total Columns: 14

---

## 🤖 Models Used

### Model 1 — Logistic Regression (Traditional ML)
- Text vectorized using TF-IDF (Term Frequency Inverse Document Frequency)
- Bigrams included (ngram_range = 1,2)
- Fast, interpretable, good baseline

### Model 2 — Transformers (Advanced AI)
- Uses pre-trained DistilBERT model from HuggingFace
- Fine-tuned on intern feedback data
- Much more accurate for understanding context

---

## 📈 Results

- Logistic Regression Accuracy: ~85 percent
- Identifies top negative departments
- Shows impact of mentor availability on satisfaction
- Predicts sentiment on any new feedback text

---

## 🎯 Outcome — Improvement Areas Identified

The model helps answer:
- Which departments have the most negative feedback?
- Does mentor availability affect intern sentiment?
- What percentage of interns would recommend the program?
- What are the most common complaints in negative reviews?

---

## 🛠️ Libraries Used

| Library | Purpose |
|---|---|
| pandas, numpy | Data handling |
| scikit-learn | Logistic Regression, TF-IDF |
| transformers | BERT / DistilBERT model |
| torch | Deep learning backend |
| matplotlib, seaborn | Visualizations |
| wordcloud | Word frequency visualization |

---

## 🚀 How to Run

1. Clone this repository
```
git clone https://github.com/yourusername/intern-sentiment-analysis
cd intern-sentiment-analysis
```

2. Install all requirements
```
pip install -r requirements.txt
```

3. Open the notebook
```
jupyter notebook intern_sentiment_analysis.ipynb
```

4. Run all cells from top to bottom

---

## 📁 Project Structure

```
intern-sentiment-analysis/
│
├── intern_sentiment_analysis.ipynb   ← Main notebook with full code
├── intern_feedback_dataset.csv       ← Dataset (300 intern records)
├── README.md                         ← Project description (this file)
└── requirements.txt                  ← All required libraries
```

---

## 👨‍💻 Author

**Your Name Here**
Data Science Intern
GitHub: github.com/yourusername

---

## 📝 Project Type

Internship Task — NLP Sentiment Classification
