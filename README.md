# Fine-tuning-with-quantization-and-lora
 
This project explores using LoRA (Low-Rank Adaptation) and quantization to fine-tune a large language model (LLM) efficiently. I used these techniques to reduce the size of a model while still maintaining accuracy, particularly focusing on predicting conversion rates from marketing SMS data. Throughout this process, I gained hands-on experience with advanced generative AI techniques, optimizing models for real-world applications.

## Overview
The goal of this project was to explore the entire lifecycle of using LLMs—from extracting meaningful features from text to fine-tuning a massive model while reducing its size using quantization and LoRA. I tackled each step by first extracting features using both traditional regex-based methods and OpenAI’s LLM. Then, I fine-tuned the Mistral LLM (14GB) and applied quantization to make the model more efficient.

## Key techniques and what I learned:

LoRA (Low-Rank Adaptation): I learned how to fine-tune large models with fewer trainable parameters, which is faster and requires less memory.
Quantization: I applied 4-bit and 8-bit quantization, learning how this reduces model size and speeds up inference without sacrificing too much accuracy.
Gradient Checkpointing: This allowed me to manage memory usage by recomputing intermediate activations, a crucial technique for working with large models on limited hardware.
k-bit Training: I experimented with training the model using lower-bit precision weights, gaining insights into how it reduces computational load while maintaining performance.
What I Did
## Feature Extraction:

I first used regex to extract features from marketing SMS messages (e.g., discounts), but when this approach proved limited, I switched to using OpenAI’s LLM, which handled nuanced cases better.

## Modeling with Mistral LLM: I used the 14GB Mistral model to predict conversion likelihoods based on the features. I learned the importance of efficient processing and how LLMs can struggle with resource-intensive tasks.

##Fine-Tuning and Optimization:

I applied LoRA to fine-tune the Mistral model using only 37.5M trainable parameters, making the process more memory-efficient.
I used quantization to reduce the model’s size by converting its weights to lower precision (4-bit and 8-bit).
Gradient checkpointing and k-bit training allowed me to optimize memory and computational efficiency during training, further reducing the resource demands.

## Key Takeaways

Working on this project taught me how to handle large models efficiently and how various tuning techniques, like LoRA and quantization, can dramatically improve their usability without needing vast computational power. I also learned how to optimize training through gradient checkpointing and k-bit training, enabling me to work with limited resources while still seeing meaningful results.


## What I Learned

This project deepened my understanding of LLMs, tuning, and model compression techniques. I now better appreciate the balance between model performance and computational efficiency. These techniques make deploying large models in real-world scenarios much more practical, especially when faced with hardware limitations.

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Keshavsingh/Fine-tuning-with-quantizationand-Lora-Project.git
2. ** Get your api keys and access token from hugging face 
3. Run the jupyter notebooks and play with your personalised trained dataset
