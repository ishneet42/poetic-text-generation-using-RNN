# 📜 Shakespeare Text Generator

This project uses a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM) layers to generate text in the style of William Shakespeare. The model is trained on a subset of Shakespeare's works and can generate new text based on the patterns it has learned.

## 📖 Overview

The model is built using TensorFlow and Keras. It takes a sequence of characters as input and predicts the next character in the sequence. The generated text can be influenced by adjusting the "temperature" parameter, which controls the randomness of the predictions.

## 📚 Dataset

The dataset used for this project is Shakespeare's text, which is available publicly. The text is preprocessed to lowercase and sliced into sequences of a fixed length to be fed into the model.

## 🏗️ Model Architecture

The model consists of the following layers:
- LSTM layer with 128 units
- Dense layer
- Activation layer with softmax function

The model is compiled with categorical crossentropy loss and the RMSprop optimizer.

## 🏋️ Training

The model is trained on sequences of 40 characters, with a step size of 3 characters between sequences. The training data is encoded as one-hot vectors.
