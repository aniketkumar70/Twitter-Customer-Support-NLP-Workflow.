# Twitter Customer Support NLP Workflow

This project is focused on preparing and analyzing a dataset of customer support conversations from Twitter, with an emphasis on Natural Language Processing (NLP) for future classification tasks.

## 📁 Dataset

- **Source:** [Kaggle - Customer Support on Twitter](https://www.kaggle.com/datasets/thoughtvector/customer-support-on-twitter)
- The dataset contains tweets from various support accounts and customers.
- It includes details such as tweet text, timestamps, user handles, and whether the tweet is from a customer or support.

## ⚙️ Workflow Steps

### 1. Data Loading
- The dataset was loaded using `pandas` from the CSV file.
- Basic inspection was performed using `.head()`, `.columns`, and `.shape`.

### 2. Data Understanding
- Checked the distribution of tweet types using `.value_counts()`.
- Visualized tweet classes using a `seaborn` bar plot to understand class imbalance.

### 3. Text Preprocessing
- Removed mentions, hashtags, URLs, punctuations, and extra whitespace.
- Applied lowercase conversion to standardize the text data.
- Used tokenization to break tweets into individual words.
- Stop words were removed using NLTK’s stopword list.

### 4. Tokenization & Padding
- Used TensorFlow's Tokenizer to vectorize the tweet texts.
- Applied padding to ensure uniform input shape for deep learning models.

## 📦 Libraries Used

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `re`, `string`
- `nltk`
- `tensorflow.keras.preprocessing.text`

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/twitter-support-nlp.git
   cd twitter-support-nlp
