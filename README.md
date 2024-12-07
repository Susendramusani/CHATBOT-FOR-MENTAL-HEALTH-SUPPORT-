# A Comparative Study of Rule-Based, Retrieval-Based & Generative Models

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

This project presents a comparative analysis of three chatbot architectures: rule-based, retrieval-based, and generative models. Each model is implemented and evaluated to understand their respective strengths and limitations in handling various conversational scenarios.

## Features

- **Rule-Based Model**: Utilizes predefined rules to generate responses, offering high precision for specific queries.
- **Retrieval-Based Model**: Employs a Long Short-Term Memory (LSTM) network to classify queries and retrieve the most relevant responses from a predefined set.
- **Generative Model**: Implements an encoder-decoder architecture with LSTMs to generate novel responses, providing flexibility in handling diverse inputs.

## Project Structure

├── data
│   ├── raw
│   ├── processed
│   └── test
├── models
│   ├── rule_based
│   ├── retrieval_based
│   └── generative
├── notebooks
├── scripts
│   ├── preprocess.py
│   ├── train_rule_based.py
│   ├── train_retrieval_based.py
│   ├── train_generative.py
│   └── evaluate.py
├── chat.py
├── requirements.txt
└── README.md
