# NeuralNetworksHomeAssignment4

Student Information

- Name: Ruthvik Reddy Gaddam
- Student ID: 700755809 RXG58090
- Course: CS5720 Neural Networks CRN-23848

## Overview

This repository contains the final submission of the home assignment 4 of the Neural Networks course. The submission topics include NLP Preprocessing Pipeline, Named Entity Recognition with SpaCy, Scaled Dot Product Attention, Sentiment Analysis using HuggingFace Transformers.

- File Structure:
- The assignment contains 4 tasks which were implemented separately in 4 python notebooks
    - ha4task1.ipynb
    - ha4task2.ipynb
    - ha4task3.ipynb
    - ha4task4.ipynb

## How to execute locally

Download the repository and install the mentioned packages in the requirements.txt file and run the cells of the Jupyter Notebook

### 1. NLP Preprocessing Pipeline

Write a Python function that performs basic NLP preprocessing on a sentence. The function should do the following steps:
1.	Tokenize the sentence into individual words.
2.	Remove common English stopwords (e.g., "the", "in", "are").
3.	Apply stemming to reduce each word to its root form.
Use the sentence:
"NLP techniques are used in virtual assistants like Alexa and Siri."
The function should print:
- A list of all tokens
- The list after stop words are removed
- The final list after stemming
Expected Output: 
Your program should print three outputs in order:
1.	Original Tokens – All words and punctuation split from the sentence
2.	Tokens Without Stopwords – Only meaningful words remain
3.	Stemmed Words – Each word is reduced to its base/root form

Short Answer Questions:
1.	What is the difference between stemming and lemmatization? Provide examples with the word “running.”
2.	Why might removing stop words be useful in some NLP tasks, and when might it actually be harmful?

## 2. Named Entity Recognition with SpaCy

Task: Use the spaCy library to extract named entities from a sentence. For each entity, print:
- The entity text (e.g., "Barack Obama")
- The entity label (e.g., PERSON, DATE)
- The start and end character positions in the string
Use the input sentence:
"Barack Obama served as the 44th President of the United States and won the Nobel Peace Prize in 2009."
Expected Output: 
Each line of the output should describe one entity detected
Short Answer Questions:
1.	How does NER differ from POS tagging in NLP?
2.	Describe two applications that use NER in the real world (e.g., financial news, search engines).

## 3. Scaled Dot Product Attention 

Task: Implement the scaled dot-product attention mechanism. Given matrices Q (Query), K (Key), and V (Value), your function should:
- Compute the dot product of Q and Kᵀ
- Scale the result by dividing it by √d (where d is the key dimension)
- Apply softmax to get attention weights
- Multiply the weights by V to get the output

Use the following test inputs:
- Q = np.array([[1, 0, 1, 0], [0, 1, 0, 1]])
- K = np.array([[1, 0, 1, 0], [0, 1, 0, 1]])
- V = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

Expected Output Description:

Your output should display:

1.	The attention weights matrix (after softmax)
2.	The final output matrix

Short Answer Questions:

1.	Why do we divide the attention score by √d in the scaled dot-product attention formula?
2.	How does self-attention help the model understand relationships between words in a sentence?


## 4. Sentiment Analysis using HuggingFace Transformers
 
Task: Use the HuggingFace transformers library to create a sentiment classifier. Your program should:
- Load a pre-trained sentiment analysis pipeline
- Analyze the following input sentence:
"Despite the high price, the performance of the new MacBook is outstanding."
- - Print:
- - Label (e.g., POSITIVE, NEGATIVE)
- - Confidence score (e.g., 0.9985)

Expected Output:

Your output should clearly display:

Sentiment: [Label]

Confidence Score: [Decimal between 0 and 1]

Short Answer Questions:
1.	What is the main architectural difference between BERT and GPT? Which uses an encoder and which uses a decoder?
2.	Explain why using pre-trained models (like BERT or GPT) is beneficial for NLP applications instead of training from scratch.

