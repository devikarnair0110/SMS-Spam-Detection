# NLP-Based SMS Spam Detection

## Project Description

This project develops an NLP-based SMS spam detection system that automatically classifies SMS messages into **Ham** and **Spam** categories.

The project uses **text preprocessing, TF-IDF feature extraction, and Multinomial Naive Bayes** for SMS classification.

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab

## Dataset

**Dataset:** SMS Spam Collection Dataset

**File:** `spam.csv`

The important columns are:

* `label` – Target variable
* `message` – SMS text

Classes:

* `0` – Ham
* `1` – Spam

## Methodology

The project follows these steps:


Dataset
   ↓
Data Cleaning
   ↓
Text Preprocessing
   ↓
TF-IDF Feature Extraction
   ↓
Multinomial Naive Bayes
   ↓
Prediction
   ↓
Evaluation


### Text Preprocessing

* Convert text to lowercase
* Remove URLs
* Remove special characters and numbers
* Tokenization
* Stopword removal
* Porter stemming

### TF-IDF

TF-IDF is used to convert cleaned SMS text into numerical feature vectors.

* Maximum features: 5,000
* N-gram range: (1, 2)

### Machine Learning Model

**Multinomial Naive Bayes** is used for SMS classification.

## Results

The model achieved:

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 96.71% |
| Precision | 98.99% |
| Recall    | 74.81% |
| F1-Score  | 85.22% |

## Sample Predictions

* "Congratulations! You have won a free prize. Call now!" → **SPAM**
* "Hey, are you coming to college tomorrow?" → **HAM**
* "You have been selected for a cash reward. Claim now!" → **SPAM**
* "Can you send me the assignment?" → **HAM**

## Project Files


NLP-SMS-Spam-Detection/
├── README.md
├── source_code.py
├── requirements.txt
├── dataset/
│   └── spam.csv
├── screenshots/
└── report/
    └── NLP_Report.docx


## Future Scope

* Use advanced NLP models such as BERT
* Use larger datasets
* Implement multilingual spam detection
* Develop a web or mobile application
* Compare different machine learning algorithms
* Improve text preprocessing

## Conclusion

The project demonstrates that traditional NLP techniques combined with machine learning can be used to effectively classify SMS messages as Ham or Spam.
