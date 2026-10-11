# ML Algorithms From Scratch

Building machine learning algorithms from scratch in Python to understand their mathematics, optimization, and internal mechanics.

The goal is to implement algorithms step by step, experiment with them, and compare them against established ML libraries.

## Algorithms

### 1. Linear Regression

**Status:** Completed

Implemented single-feature and multivariable Linear Regression using pure Python.

**Concepts covered:**
- Linear models, weights, and bias
- Mean Squared Error (MSE)
- Gradient calculation
- Batch gradient descent
- Iterative parameter optimization
- Dynamic support for multiple input features

**Model:**

$$
\hat{y} = \sum_{j=1}^{d} w_j x_j + b
$$
**Experiment:** Trained a model on 20 examples with five features, recovering weights close to the known parameters.

| Metric | Result |
|---|---:|
| Features | 5 |
| Samples | 20 |
| Epochs | 10,000 |
| Learning rate | 0.01 |
| Training MSE | 0.00544 |

### 2. Logistic Regression

**Status:** Core implementation completed

Implemented single-feature binary Logistic Regression by adapting my Linear Regression algorithm.

**Concepts:** Sigmoid, probability prediction, binary cross-entropy, gradients, batch gradient descent, and decision boundaries.

**Key equations:**

```text
z = wx + b
p = 1 / (1 + e^(-z))
dw = mean((p - y) * x)
db = mean(p - y)
```

**Experiment results:**

| Metric | Value |
|---|---:|
| Features | 1 |
| Samples | 20 |
| Epochs | 10,000 |
| Learning rate | 0.06 |
| Final weight | 0.908613 |
| Final bias | -4.193241 |
| Average loss across epochs | 0.401921 |

Next: evaluate predictions, test on unseen data, and compare with Scikit-learn.

## Roadmap

- [ ] Multivariable Logistic Regression
- [ ] K-Nearest Neighbors
- [ ] Decision Trees
- [ ] Naive Bayes
- [ ] Support Vector Machines
- [ ] K-Means Clustering
- [ ] Random Forest
- [ ] Neural Networks from scratch
- [ ] Backpropagation and automatic differentiation

## Tech Stack

- **Language:** Python
- **Core:** Pure Python and standard library
- **Comparison:** Scikit-learn where useful

## Learning Approach

For every algorithm:

1. Understand the intuition.
2. Learn the mathematics.
3. Implement from scratch.
4. Experiment with data and hyperparameters.
5. Evaluate and compare results.

## Long-Term Goal

Build a strong foundation in machine learning and deep learning by understanding algorithms from the ground up.

---

*Learning by implementing. Understanding by experimenting.*
