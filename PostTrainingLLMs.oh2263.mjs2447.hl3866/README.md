# Post Training for LLMs

This repository contains a hands-on implementation of **post-training techniques for Large Language Models (LLMs)** using **Proximal Policy Optimization (PPO)**. The code demonstrates how reinforcement learning can be applied to fine-tune LLMs, aligning them more closely with desired behaviors, safety constraints, or user feedback.

## Overview

The notebook [`PostTraining_using_PPO.ipynb`](./PostTraining_using_PPO.ipynb) walks through the following:

- Loading a pre-trained language model and tokenizer
- Defining custom reward functions
- Implementing PPO for language model fine-tuning
- Training and evaluating the model post-finetuning

This approach is commonly used in the **RLHF (Reinforcement Learning with Human Feedback)** pipeline for aligning models like GPT with human preferences.

## Key Features

- Uses Hugging Face's `transformers` and `trl` libraries  
- Demonstrates policy optimization using PPO  
- Custom reward function integration  
- Includes comparison between trained and post-trained model outputs  

## Setup

To run the notebook, install the following dependencies:

```bash
pip install transformers datasets accelerate peft trl torch
```

## File Structure

```
├── PostTraining_using_PPO.ipynb   # Main notebook with PPO-based post-training code
├── README.md                      # Project documentation
```

## Example Use-Case

The notebook showcases how to take a pre-trained model like `distilbert` or `gpt2`, define a simple reward (e.g., based on sentiment or length), and fine-tune it using PPO to encourage certain response behaviors.

## Models Used

- `gpt2` (as the language model)
- Optional: sentiment models for reward shaping
