
# Toxic Text Classification with LSTM

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

This project implements a Long Short-Term Memory (LSTM) model for classifying toxic comments into multiple categories, including `toxic`, `severe_toxic`, `obscene`, `threat`, `insult`, and `identity_hate`. The model is built using PyTorch and is trained on the Jigsaw Toxic Comment Classification Challenge dataset.

---

## 📁 Project Structure

```
toxic_text_lstm/
├── .gitattributes             # Git attributes for handling line endings and merge strategies
├── requirements.txt           # Python dependencies for the project
├── train.csv                  # Dataset for training the model (ensure this file is included)
├── toxic_classifier.ipynb     # Jupyter Notebook for training and evaluating the model
└── README.md                  # Project overview and setup instructions
```

---

## 🔧 Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/Bikram-ghuku/toxic_text_lstm.git
   cd toxic_text_lstm
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dataset**

   - Download `train.csv` from [Kaggle](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data)
   - Place it in the project root directory

---

## 🧹 Preprocessing

The preprocessing steps include:

- Cleaning the text (removing punctuation, converting to lowercase, etc.)
- Tokenizing the text using 216477 tokens
- Encoding the sentences
- Balancing the dataset using upsampling

These steps are implemented in the `toxic_classifier.ipynb` notebook.

---

## 🏋️ Training

To train the model:

1. Open the `toxic_classifier.ipynb` notebook.
2. Follow the instructions within the notebook to preprocess the data, define the model, and train it.

The notebook provides a step-by-step guide for training the LSTM model.

---

## 🔍 Inference

After training the model, you can use it to classify new comments. The inference code is also included in the `toxic_classifier.ipynb` notebook.

---

## 📊 Results

- **F1 Score (micro):** 0.8178  
- **Accuracy Score:** 0.9142


---

## 🙌 Acknowledgments

- [Kaggle Jigsaw Toxic Comment Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
- PyTorch Team
