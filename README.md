# Chatbot for Mental Health Support

## Overview

This repository contains the implementation and analysis of three chatbot architectures—**Rule-Based**, **Retrieval-Based**, and **Generative Models**—designed to provide mental health support. These models are trained on a dataset of mental health FAQs and evaluated using various quantitative and qualitative metrics to determine their effectiveness, flexibility, and suitability for real-world applications.

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Features](#features)  
3. [Technologies Used](#technologies-used)  
4. [Dataset](#dataset)  
5. [Model Descriptions](#model-descriptions)  
6. [Usage](#usage)  
7. [Evaluation Metrics](#evaluation-metrics)  
8. [Results](#results)  
9. [Future Work](#future-work)  
10. [Contributing](#contributing)  

---

## Introduction

The project explores the trade-offs between precision, fluency, and adaptability of three chatbot models to assist individuals seeking mental health support. These systems aim to address challenges such as scalability, empathy, and response relevance, critical for effective mental health care applications.

---

## Features

- **Rule-Based Model:** Precise responses for structured queries using pre-defined rules.
- **Retrieval-Based Model:** Flexible responses by matching user queries with a pre-built response database.
- **Generative Model:** Adaptive and natural language responses leveraging neural networks.
- Comparative analysis of models based on **accuracy**, **BLEU score**, and **perplexity**.
- Implementation of preprocessing techniques like tokenization, stopword removal, and sequence padding.

---

## Technologies Used

- **Programming Language:** Python  
- **Frameworks:** TensorFlow, Keras  
- **Libraries:** NLTK for preprocessing, NumPy for computations  
- **Hardware:** NVIDIA GPU for accelerated model training  

---

## Dataset

The dataset consists of **1,000 question-answer pairs** related to mental health topics. Each entry includes:
- A unique ID
- A question text
- An answer text

### Preprocessing
- **Tokenization:** Divides text into words or phrases.
- **Stopword Removal:** Filters out common but uninformative words.
- **Sequence Padding:** Ensures uniform sequence length for compatibility with models.

---

## Model Descriptions

1. **Rule-Based Model**  
   - **Approach:** Bag-of-Words with TF-IDF weighting and cosine similarity for response matching.
   - **Strengths:** High precision for structured inputs.
   - **Weaknesses:** Poor adaptability to complex or novel queries.

2. **Retrieval-Based Model**  
   - **Architecture:** LSTM-based neural network for classification.
   - **Strengths:** Balances precision and relevance for in-domain queries.
   - **Weaknesses:** Limited flexibility for unseen inputs.

3. **Generative Model**  
   - **Architecture:** Encoder-Decoder with LSTMs.
   - **Strengths:** Handles diverse and nuanced queries.
   - **Weaknesses:** Risk of incoherent or irrelevant outputs due to limited training data.

---

## Usage

1. Preprocess the dataset:
   ```bash
   python preprocess.py

2. Train models:
   Rule-Based:
   python rule_based_model.py
   Retrieval-Based:
   python retrieval_based_model.py
   Generative:
   python generative_model.py

3.Evaluate models:
   python evaluate.py

## Evaluation Metrics
  - **Accuracy:** Measures the proportion of correct responses.
  - **BLEU Score:** Assesses fluency and relevance for generative models.
  - **Perplexity:** Indicates the coherence of generative responses.
## Results

| Model             | Accuracy (%) | BLEU Score | Perplexity |
|--------------------|--------------|------------|------------|
| Rule-Based        | 72.3         | N/A        | N/A        |
| Retrieval-Based   | 85.4         | N/A        | N/A        |
| Generative        | N/A          | 24.5       | 12.7       |

## Future Work
  -1.Hybrid Models: Combine retrieval-based and generative models for better accuracy and flexibility.
  
  -2.Attention Mechanisms: Use transformer architectures to improve response coherence.
  
  -3.Larger Datasets: Pretrain models on diverse datasets to enhance generalization.

## Contributing
  -Contributions are welcome! Please fork the repository and create a pull request with your enhancements or fixes.
