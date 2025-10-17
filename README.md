# MiniLM French Sentiment Analysis

This project demonstrates how to use **MiniLM embeddings** to classify French text sentiment as **positive** or **negative**.  
It was developed and executed entirely in **Kaggle**.

---

## Project Overview
- Convert French tweets into **MiniLM embeddings** using the `Transformers` library.
- Visualize embeddings with **PCA** and **t-SNE**.
- Train a deep neural network to classify sentiment.
- Deploy a simple user interface with **Gradio** to:
  - Enter a tweet and get its sentiment.
  - Upload a `.txt` file and get predictions for each line.

---

## Tech Stack
- Python
- NumPy, Pandas, Matplotlib, Seaborn
- Scikit-learn
- TensorFlow / Keras
- Transformers (MiniLM model)
- Gradio

---

## How It Works
1. **Data Preprocessing**
   - Clean and balance the dataset of French tweets.
   - Remove URLs, mentions, hashtags, and special characters.

2. **Embedding Generation**
   - Load the `sentence-transformers/all-MiniLM-L12-v2` model.
   - Convert tweets into numerical embeddings.

3. **Visualization & Modeling**
   - Apply PCA and t-SNE to visualize the embeddings.
   - Train a dense neural network classifier on top of the embeddings.

4. **Deployment**
   - Build a Gradio interface to test the model with text or uploaded files.

---

## Installation

```bash
# Clone the repository
git clone https://github.com/malek-messaoudii/MiniLM-Embedding.git

# Navigate to the project directory
cd MiniLM-Embedding.git

# Install dependencies
pip install -r requirements.txt
