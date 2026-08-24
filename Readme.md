# Next Word Prediction using LSTM

A deep learning application that predicts the next word in a sentence using an **LSTM (Long Short-Term Memory)** neural network. The application provides an interactive Streamlit interface where users can enter text and generate next-word predictions.

## Live Demo

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://nextwordprediction-j6wpksla3cgkywcf7vp2yz.streamlit.app/)

**Try the application:**
https://nextwordprediction-j6wpksla3cgkywcf7vp2yz.streamlit.app/

## Features

* Predicts the next word based on user input
* Uses an LSTM neural network for text prediction
* Text preprocessing using a tokenizer
* Interactive Streamlit web interface
* Loads a pre-trained LSTM model
* Simple and user-friendly interface

## Technologies Used

* **Python**
* **TensorFlow / Keras**
* **LSTM**
* **NumPy**
* **Streamlit**
* **Pickle**

## How It Works

The application follows these main steps:

1. The user enters a sentence or sequence of words.
2. The tokenizer converts the input text into numerical sequences.
3. The sequence is padded to match the input length expected by the model.
4. The trained LSTM model processes the sequence.
5. The model predicts the probability of the next word.
6. The predicted word is displayed in the Streamlit interface.

## Project Structure

```text
next_word/
│
├── app.py
├── lstm_model.h5
├── tokenizer.pkl
├── max_len.pkl
├── qoute_dataset.csv
├── requirements.txt
├── .gitignore
└── README.md
```

## Model

The project uses an **LSTM (Long Short-Term Memory)** neural network, which is designed to learn patterns and dependencies in sequential data such as text.

The trained model is saved as:

```text
lstm_model.h5
```

The tokenizer used during training is stored in:

```text
tokenizer.pkl
```

The maximum sequence length used by the model is stored in:

```text
max_len.pkl
```

## Running Locally

Clone the repository:

```bash
git clone <your-github-repository-url>
cd next_word
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run the Streamlit application:

```bash
streamlit run app.py
```

The application will then be available in your browser.

## Deployment

The application is deployed using **Streamlit Community Cloud**. Streamlit Community Cloud connects to a GitHub repository and automatically deploys the Streamlit application. Changes pushed to the repository can also trigger updates to the deployed application.

## Future Improvements

* Predict multiple words instead of only one word
* Improve prediction accuracy with a larger dataset
* Experiment with GRU and Transformer-based models
* Add top-k word predictions with probabilities
* Improve the user interface
* Fine-tune the model using a larger text corpus
