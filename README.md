# Turkish NLP: Optimization Algorithm Analysis

This project evaluates the performance of different optimization algorithms (GD, SGD, and Adam) on a Turkish text classification task. It uses semantic embeddings to train a regression model that distinguishes between "good" and "bad" answers to specific questions.

## 🚀 Project Overview

The core objective is to analyze how different optimizers affect the training process of a single-layer regression model (and optionally an MLP) using Turkish language data.

- **Embedding Model:** `ytu-ce-cosmos/turkish-e5-large` (used to transform text into 1024-dimensional vectors).
- **Classification Task:** Predicting whether an answer is correct (+1) or incorrect (-1) based on the question-answer pair.
- **Optimizers Compared:** - Gradient Descent (GD)
  - Stochastic Gradient Descent (SGD)
  - Adam

## 📊 Key Features

### 1. Performance Comparison
The project includes detailed visualizations of:
- **Epoch vs. Loss/Accuracy:** How the model learns over iterations.
- **Time vs. Loss/Accuracy:** Computation efficiency of each algorithm.
- Comparison across 5 different initial weight sets to ensure robustness.

### 2. Weight Trajectory Visualization (t-SNE)
Using **t-SNE**, the high-dimensional weight vectors ($2d+1$) are reduced to 2D space to visualize the optimization paths. This helps in understanding how different optimizers navigate the loss landscape from various starting points.
