# 📝 Next Word Prediction using LSTM & GRU (Hamlet – Shakespeare )

This is an end-to-end **Next Word Prediction** project built with **TensorFlow**, **Keras**, and **Streamlit**.  
It predicts the next word based on context learned from **Hamlet** by *William Shakespeare*, downloaded from the **NLTK Gutenberg corpus**.

The project includes:
- Tokenization
- LSTM & GRU model training
- Model + tokenizer saving
- A Streamlit web interface for prediction

---

## 📚 Dataset

The dataset comes from the **NLTK Gutenberg collection**.

```python
from nltk.corpus import gutenberg
data = gutenberg.raw('shakespeare-hamlet.txt')

```

## Why Hamlet?

Rich, classic English text

Large enough for training

Excellent for NLP sequence prediction tasks


## Project Structure 
```
## next-word-prediction/
│── app.py
│── nextword_model.h5
│── tokenizer.pickle
│── requirements.txt
│── README.md
│── experiment.ipynb
│── .gitignore
```

## 🧠 Model Details

The model is a word-level LSTM & GRU designed to learn patterns in Shakespearean language.

Files:

nextword_model.h5 → Trained model

tokenizer.pickle → Saved tokenizer

Both must be placed in the same folder 

## 🔧 Training Process (Summary)

Load Hamlet text

tokenize text

Create input sequences

Pad sequences

Train an LSTM model

Train an GRU model

Save:

The trained model (nextword_model.h5)

The tokenizer (tokenizer.pickle)


## 🚀 How to Run the Project 

1. Clone the Repository
```
git clone https://github.com/UTSAVPANCHAL2006/Next-Word-Prediction.git

cd next-word-prediction

```
2. Create Virtual Environment (Python 3.10 recommended)
```
python3.10 -m venv venv
source venv/bin/activate
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Run Streamlit App
```
streamlit run app.py
```
