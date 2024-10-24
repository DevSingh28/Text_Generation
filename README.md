# GPT-like Text Generation Model Using Transformer Architecture

This project demonstrates a GPT-like text generation model using the Transformer architecture. The model is trained on a small subset of the DailyDialog dataset to showcase the functionality of Transformer-based text generation. Due to limited resources, the model is trained on a very small dataset and cannot generate fully accurate or meaningful responses, but it serves as a practical example of how the architecture works.

## Model Overview

The model uses a simplified version of the GPT architecture:
- An embedding layer to convert characters into dense vectors.
- Positional encoding to capture the order of the sequence.
- A multi-layer Transformer encoder to process the input sequence.
- A fully connected output layer to predict the next character in the sequence.

## Dataset

The model is trained on the [DailyDialog dataset](https://huggingface.co/datasets/daily_dialog), specifically using a 10% subset of the training data for demonstration purposes. The dialogues are tokenized into individual characters.

## Model Features

- Transformer architecture with 2 encoder layers.
- Trained to predict the next character in a sequence of length 12.
- Character-level text generation based on a prompt input.

## Requirements

Install the required Python packages using the following command:
```bash
pip install -r requirements.txt

torch==2.0.1
datasets==2.15.1
tqdm==4.66.1
gradio==4.36.0
numpy==1.24.3
