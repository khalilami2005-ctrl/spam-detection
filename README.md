# spam-detection

# Spam Email Classifier (Machine Learning)

## Description

This project is a simple **machine learning spam classifier** built with Python.

The program trains a model to classify messages as:

* **Spam**
* **Ham (not spam)**

It uses **Naive Bayes** and **text vectorization** to learn patterns from labeled email messages.

---

## Technologies Used

* Python
* pandas
* scikit-learn

Machine learning techniques used:

* CountVectorizer (text → numerical vectors)
* Multinomial Naive Bayes (classification)

---

## How It Works

1. The program loads a dataset of emails.
2. The email text is converted into numerical vectors using **CountVectorizer**.
3. The dataset is split into:

   * Training data (80%)
   * Testing data (20%)
4. A **Naive Bayes classifier** is trained.
5. The model predicts whether a new message is spam or not.

---

## Dataset Format

The dataset file (`emails.csv`) must contain two columns:

| text          | spam   |
| ------------- | ------ |
| email content | 0 or 1 |

Where:

* **1 = Spam**
* **0 = Ham**

Example:

text,spam
"Win a free iPhone now",1
"Hello how are you",0

---

## Installation

Clone the repository:

git clone https://github.com/yourusername/spam-email-classifier.git

Move into the project folder:

cd spam-email-classifier

Install dependencies:

pip install pandas scikit-learn

---

## Running the Program

Run the Python script:

python spam_classifier.py

Then enter a message to test the classifier.

Example:

Enter your message:
You won a free vacation

Output:

Spam

---

## Machine Learning Model

The classifier uses:

* **CountVectorizer** to convert text into numerical features
* **Multinomial Naive Bayes** for probabilistic classification

This model is commonly used for:

* Spam detection
* Sentiment analysis
* Document classification

---

## Example Output

Accuracy: 0.96

Enter your message:
Hello my friend

Prediction: Ham

---

## Project Structure

spam-email-classifier
│
├── spam_classifier.py
└── README.md

---

## Author

Machine Learning practice project using Python.
