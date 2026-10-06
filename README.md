# Next Word Prediction using LSTM

## Project Overview

This project develops a Next Word Prediction model using an LSTM (Long Short-Term Memory) neural network. The model is trained on the Tiny Shakespeare dataset to learn word patterns and predict the next word from a given text sequence.

## Objective

The main objective of this project is to build a deep learning model that can understand sequential text patterns and predict the most likely next word.

## Dataset

**Dataset:** Tiny Shakespeare  
**Source:** TensorFlow Datasets

The dataset contains Shakespeare's text and is used to train the model to learn language patterns.

## Technologies Used

- Python
- TensorFlow
- Keras
- TensorFlow Datasets
- NumPy
- Matplotlib
- LSTM

## Project Workflow

1. Load the Tiny Shakespeare dataset
2. Preprocess the text
3. Tokenize the text
4. Convert words into numerical sequences
5. Create fixed-length sequences
6. Apply padding
7. Build the LSTM model
8. Train the model
9. Evaluate training and validation performance
10. Predict the next word

## Model Architecture

The model consists of:

- **Embedding Layer** – Converts word IDs into numerical vector representations.
- **LSTM Layer** – Learns sequential patterns and context from previous words.
- **Dense Layer with Softmax** – Predicts the probability of each possible next word.

### Architecture

`Input → Embedding → LSTM → Dense + Softmax → Next Word`

## Training

The model was trained for **5 epochs** with a batch size of **64**.

### Performance

- Training Accuracy: **11.82%**
- Validation Accuracy: **9.28%**



## Results

The training accuracy increased during training, showing that the model learned patterns from the training data. The validation results also showed that the model was able to learn some general patterns from unseen data.

The model showed some tendency toward overfitting as the validation loss increased in later epochs.

## Conclusion

This project demonstrates how LSTM networks can be used for next-word prediction. The model learned sequential patterns from the Tiny Shakespeare dataset and generated next-word predictions for different input phrases.

The performance could be improved using a larger model, more training data, dropout, early stopping, hyperparameter tuning, and longer training with suitable regularization.

## Project Files

- `Next_Word_Prediction_LSTM.ipynb` – Jupyter Notebook containing the complete project.

