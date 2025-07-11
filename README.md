# 📘 README: Perceptron Logic Gate Classifier

## 🔍 Overview

This is a simple implementation of a **Perceptron** from scratch using NumPy and Matplotlib in Python. The code demonstrates how a single-layer perceptron can learn to classify **AND gate** outputs. It also plots **true vs predicted outputs** during each training epoch to visually show the learning progress.

## 🧠 What is a Perceptron?

A Perceptron is the most basic type of neural network, used for **binary classification**. It makes decisions by calculating a weighted sum of input features, adding a bias, and passing the result through an **activation function** (in this case, a step function).

## 🛠️ Code Breakdown

- **Input (`X`)**: 4 combinations for 2-input gates: `[[0,0], [0,1], [1,0], [1,1]]`
- **Labels (`y`)**: The output of the AND gate for each input.
- **Weights (`w`)**: Randomly initialized, updated through learning.
- **Activation Function**: Step function returns `1 if z > 0`, else `0`.
- **Training**: 20 epochs using simple Perceptron learning rule.
- **Visualization**: Plots **True vs Predicted** outputs for every epoch.

## ▶️ How to Run

Make sure you have Python installed along with NumPy and Matplotlib.

```bash
pip install numpy matplotlib
```

Then run the Python script:

```bash
python perceptron_and_gate.py
```

## 📊 Output

At each epoch, you'll see:

- Printed **True and Predicted values**
- A plot showing the prediction progress for the 4 input samples

## 🧪 Truth Tables for Logic Gates

| Input A | Input B | AND | OR  | NAND | NOR | XOR |
|--------:|--------:|----:|----:|-----:|----:|----:|
|   0     |    0    |  0  |  0  |  1   |  1  |  0  |
|   0     |    1    |  0  |  1  |  1   |  0  |  1  |
|   1     |    0    |  0  |  1  |  1   |  0  |  1  |
|   1     |    1    |  1  |  1  |  0   |  0  |  0  |

## ⚠️ Note

- The **Perceptron** can **only solve linearly separable problems**. So, it works for AND, OR, NAND, NOR — **but not XOR**, which is not linearly separable.
- To solve XOR, you need a **multi-layer perceptron (MLP)**.

## 📁 File Structure

```
perceptron_and_gate.py     # Python script with perceptron logic
README.md                  # This file
```

## 🧩 Extensions (Ideas for You)

- Modify the labels `y` to try **OR**, **NAND**, or **NOR** gates.
- Plot the **decision boundary** (for visual understanding).
- Implement a **Multi-layer Perceptron (MLP)** to solve **XOR** gate.
- Add accuracy tracking or loss function graphs.

## 🧮 Math Essentials for Perceptron Understanding

To truly understand how a Perceptron works, it's important to grasp a few key mathematical concepts:

### ✅ Key Concepts

- **Vectors and Dot Product**: A perceptron computes the weighted sum using the dot product between the input vector and weight vector.
- **Linear Equation**: The perceptron makes decisions based on the equation `z = w.x + b`, where `z` is the weighted sum, `w` is weights, `x` is inputs, and `b` is bias.
- **Step Function**: A basic activation function which returns 1 if the weighted sum is positive, else returns 0.
- **Gradient & Error Update**: Weights are updated using the formula: `w = w + learning_rate * error * x`, and bias: `b = b + learning_rate * error`.

These concepts form the core of Perceptron logic and are foundational for understanding more complex neural networks and gradient-based learning in deep learning.

### 📗 Math Tools Covered in the Jupyter Notebook

Refer to the accompanying `Math_essentials.ipynb` for these covered topics:

- Mean, Variance, Standard Deviation
- Derivatives and Gradients
- Dot Product and Matrix Multiplication
- Simple Linear Functions
- Gradient Descent Introduction

🎯 **Goal:** Build a strong foundation in essential math to help with debugging, architecture design, and further neural network understanding.