# Custom Byte Pair Encoding (BPE) Tokenizer from Scratch

## Project Overview

This project implements a simple Byte Pair Encoding (BPE) tokenizer using Python. The tokenizer learns the most frequent character pairs from a text corpus and merges them iteratively to create subword tokens. BPE is widely used in modern Natural Language Processing (NLP) models such as GPT, BERT, and LLaMA.

## Objectives

- Read a text corpus.
- Build an initial vocabulary.
- Learn merge rules using Byte Pair Encoding.
- Encode words into subword tokens.
- Decode subword tokens back into text.

## Features

- Reads text from `corpus.txt`
- Creates character-level vocabulary
- Finds the most frequent symbol pairs
- Learns merge rules automatically
- Encodes words into subword tokens
- Decodes tokens back into words
- Displays the final vocabulary and merge rules

## Technologies Used

- Python
- Collections (`Counter`)
- Regular Expressions (`re`)

## Project Structure

```text
BPE_Tokenizer/
├── corpus.txt
├── bpe_tokenizer.py
└── README.md
```

## Workflow

1. Read the corpus.
2. Create the initial vocabulary.
3. Find frequent character pairs.
4. Merge the best pairs.
5. Learn merge rules.
6. Encode words.
7. Decode words.

## Applications

- GPT
- BERT
- LLaMA
- Machine Translation
- Text Generation
- Chatbots

## Conclusion

The Byte Pair Encoding tokenizer efficiently converts words into subword tokens by learning frequent character pair merges. This reduces vocabulary size while handling unknown words effectively, making it suitable for modern NLP applications.

# Autoregressive Causal Language Model

## Project Overview

This project implements a simplified Autoregressive Causal Language Model using NumPy. The model predicts the next token in a sequence using only previously generated tokens. The input token IDs are obtained from the Byte Pair Encoding (BPE) tokenizer.

## Objectives

- Use BPE token IDs as input.
- Create input-target pairs.
- Generate embeddings.
- Apply positional encoding.
- Apply causal masking.
- Compute self-attention.
- Predict the next token.

## Features

- Input-target pair generation
- Embedding layer
- Positional Encoding
- Causal Mask
- Self-Attention mechanism
- Linear Layer
- Softmax function
- Cross Entropy Loss
- Next Token Prediction

## Technologies Used

- Python
- NumPy

## Project Structure

```text
Autoregressive_Model/
├── autoregressive_model.py
└── README.md
```

## Workflow

1. Read token IDs.
2. Create input-target pairs.
3. Generate embeddings.
4. Add positional encoding.
5. Apply causal mask.
6. Compute self-attention.
7. Apply the linear layer.
8. Apply the Softmax function.
9. Calculate Cross Entropy Loss.
10. Predict the next token.

## Pipeline

```text
Raw Text
   ↓
BPE Tokenizer
   ↓
Token IDs
   ↓
Input-Target Pairs
   ↓
Embedding
   ↓
Positional Encoding
   ↓
Causal Mask
   ↓
Self-Attention
   ↓
Linear Layer
   ↓
Softmax
   ↓
Next Token Prediction
   ↓
Cross Entropy Loss
   ↓
Backpropagation
   ↓
Generated Text
```

## Applications

- GPT
- Chatbots
- AI Assistants
- Text Completion
- Language Modeling
- Text Generation

## Conclusion

This project demonstrates the basic workflow of an Autoregressive Causal Language Model. It combines BPE tokenization, embeddings, positional encoding, causal masking, and self-attention to predict the next token in a sequence.
