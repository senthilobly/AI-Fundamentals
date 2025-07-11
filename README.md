# Python-Refresher
Python Fundamentals and Numpy Library uses in Machine Learning models

# Python Learning Notebooks

This repository contains beginner-to-intermediate level Jupyter notebooks designed for hands-on learning of Python programming and data manipulation using NumPy. These notebooks serve as foundational material for those entering the world of data science, machine learning, or general-purpose programming in Python.

---

## Contents

### 1. `Python_fundamentals.ipynb`

This notebook introduces the core basics of Python:

- Variables, Data Types (int, float, str, bool)
- Lists, Tuples, Sets, and Dictionaries
- Conditional statements and loops
- Functions and lambda expressions
- Basic I/O and error handling

**Goal:** Build a solid base in Python syntax and logic for any programming or data science task.

---

### 2. `Numpy_functions_uses.ipynb`

This notebook is focused on practical uses of NumPy, the essential library for numerical computing:

- Creating arrays (`np.array`, `np.arange`, `np.linspace`)
- Array operations (indexing, slicing, reshaping)
- Mathematical functions (`np.mean`, `np.std`, `np.sum`)
- Broadcasting and vectorized operations
- Linear algebra with NumPy (`np.dot`, `np.linalg`)
- Utility functions (`np.argmax`, `np.argmin`, `np.histogram`, `np.percentile`, etc.)

**Goal:** Learn how to use NumPy efficiently for numerical tasks and prepare for machine learning workflows.

---

## 3. Math Essentials for Understanding

To truly understand how a neural network works, it's important to grasp a few key mathematical concepts:

### Key Concepts

- **Vectors and Dot Product**: A neural network computes the weighted sum using the dot product between the input vector and weight vector.
- **Linear Equation**: The neural network makes decisions based on the equation `z = w.x + b`, where `z` is the weighted sum, `w` is weights, `x` is inputs, and `b` is bias.
- **Step Function**: A basic activation function which returns 1 if the weighted sum is positive, else returns 0.
- **Gradient & Error Update**: Weights are updated using the formula: `w = w + learning_rate * error * x`, and bias: `b = b + learning_rate * error`.

These concepts form the core of neural network logic and are foundational for understanding more complex neural networks and gradient-based learning in deep learning.

### Math Tools Covered in the Jupyter Notebook

Refer to the accompanying `Math_essentials.ipynb` for these covered topics:

- Mean, Variance, Standard Deviation
- Derivatives and Gradients
- Dot Product and Matrix Multiplication
- Simple Linear Functions
- Gradient Descent Introduction

**Goal:** Build a strong foundation in essential math to help with debugging, architecture design, and further neural network understanding.

## 🛠 Requirements

- Python 3.7+
- Jupyter Notebook or JupyterLab
- Packages:
  - `numpy`
  - 'matplotlib'

You can install dependencies via:
```bash
pip install numpy jupyter

