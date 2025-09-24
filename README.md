# Dialogue Summarization Using Finetuned Approach

This repository contains code and experiments for dialogue summarization using finetuned models. The approach focuses on leveraging state-of-the-art NLP techniques to generate concise and coherent summaries from conversational datasets.

## Problem Statement

In this implementation, we tackle a real-world problem: automatic dialogue summarization. Given conversational data, we want our model to generate concise, accurate summaries that capture the key points and outcomes of discussions.

### Why Dialogue Summarization?

- **Business Applications:** Meeting summaries, customer service interactions
- **Healthcare:** Doctor-patient consultation summaries
- **Education:** Lecture and discussion summarization
- **Legal:** Deposition and hearing summaries

## Dataset: DialogSum

We use the DialogSum dataset, which contains:

- **13,460 dialogues** with human-annotated summaries
- **Real-world scenarios:** Customer service, meetings, casual conversations
- **Average dialogue length:** 67.9 tokens
- **Average summary length:** 23.8 tokens

**Example from the dataset:**

```
Dialogue: "#Person1#: I think it would be a good idea if you could do some research on that company before you have the interview. #Person2#: Yeah, you're right. I should prepare more for the interview."
Summary: "#Person2# agrees with #Person1# to do more research on the company before the interview."
```

## Features

- Fine-tuning on custom dialogue datasets
- Model training and evaluation scripts
- Preprocessing utilities for dialogue data
- Example notebooks for inference and testing

## Getting Started

### Prerequisites

- Python 3.8+
- PyTorch / TensorFlow (depending on your framework)
- HuggingFace Transformers (if using)

### Installation

Clone the repository:
```bash
git clone https://github.com/ShravanNaik/Dialogue-Summarization-Using-Finetuned-Approach.git
cd Dialogue-Summarization-Using-Finetuned-Approach
```

Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage

To train a model:
```bash
python train.py --config configs/your_config.yaml
```

To generate summaries:
```bash
python summarize.py --input data/sample_dialogues.txt --output summaries.txt
```



