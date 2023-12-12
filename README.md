# Language_Translator

This Python project implements a language translator based on neural networks. It translates Sanskrit text to English using a deep learning model.

## Overview

The project involves the following steps:

1. **Reading and Preprocessing:**
   - Reading Sanskrit and English text files.
   - Text pre-processing, including removing punctuation and newline characters.

2. **Data Analysis:**
   - Analyzing the number of unique words, vocabulary size, and average sentence length in both languages.

3. **Tokenization:**
   - Tokenizing the text using the Keras Tokenizer to represent words as numerical sequences.

4. **Padding:**
   - Adding padding to sequences to ensure uniform length for input to the neural network.

5. **Model Architecture:**
   - Implementing a neural network model with an embedding layer, LSTM layer, and dense layer.

6. **Training the Model:**
   - Training the model on the preprocessed data.

7. **Evaluation:**
   - Evaluating the model's accuracy on the training set.

8. **Text-to-Speech (TTS):**
   - Implementing Text-to-Speech functionality for both English and Sanskrit translations.
   - Generating audio files for translated text.

## Usage

1. **Installation:**
   - Install the required Python packages:
     ```bash
     %pip install numpy keras tensorflow pyttsx3 gtts pygame
     ```

2. **Data Preparation:**
   - Prepare Sanskrit and English text files for training (e.g., `Sanskrit.txt` and `English.txt`).

3. **Training:**
   - Run the training script:
     ```bash
     python train_model.py
     ```

4. **Translation:**
   - Use the translation script to translate Sanskrit text to English:
     ```bash
     python translate.py --input "your_sanskrit_text_here"
     ```

5. **Text-to-Speech:**
   - Generate audio files for translated text:
     ```bash
     python text_to_speech.py --index 167
     ```

## Files and Directories

- `train_model.py`: Script for training the neural network model.
- `translate.py`: Script for translating Sanskrit text to English.
- `text_to_speech.py`: Script for generating Text-to-Speech output.
- `model/Final_LSTM.h5`: Pre-trained model file.

## Dependencies

- Python 3.x
- Libraries: numpy, keras, tensorflow, pyttsx3, gtts, pygame

## Acknowledgments

- The project is inspired by the need for Sanskrit-to-English translation using neural networks.
- Special thanks to the Keras and TensorFlow communities for providing powerful tools for deep learning.

Feel free to contribute, report issues, or provide suggestions!
