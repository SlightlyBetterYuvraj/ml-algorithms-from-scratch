# ML Algorithms From Scratch

Implementing machine learning algorithms from scratch in Python to understand the underlying mathematics, optimization, and mechanics behind them.

This repository is a hands-on learning project focused on understanding **how machine learning algorithms work internally**, rather than relying entirely on prebuilt libraries.

The goal is to build each algorithm step by step, understand the math behind it, experiment with its behavior, and eventually compare custom implementations against established ML libraries.

## Algorithms

### 1. Linear Regression

**Status:** Completed

Implemented single-feature and multivariable linear regression using pure Python.

**Concepts covered:**
- Linear models, weights, and bias
- Mean Squared Error (MSE)
- Gradient calculation
- Batch gradient descent
- Iterative parameter optimization
- Dynamic support for multiple input features

**Model:**

ŷ = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

**Experiment:** Trained a model on 20 examples with five features, recovering weights close to the known parameters.

| Metric | Result |
|---|---:|
| Features | 5 |
| Training examples | 20 |
| Epochs | 10,000 |
| Learning rate | 0.01 |
| Training MSE | 0.00544 |

The experiment used synthetic data generated from a known linear equation to verify the learned parameters.

## Planned Algorithms

- [ ] Logistic Regression
- [ ] K-Nearest Neighbors (KNN)
- [ ] Decision Tree Classifier
- [ ] Naive Bayes
- [ ] Support Vector Machine (SVM)
- [ ] K-Means Clustering
- [ ] Random Forest
- [ ] Neural Network from scratch
- [ ] Backpropagation and automatic differentiation

This roadmap will evolve as I learn new concepts and explore more advanced algorithms.

## Tech Stack

- **Language:** Python
- **Dependencies:** None for the initial linear regression implementation
- **Approach:** Mathematical implementation before library-based usage

Future algorithms may introduce NumPy or other tools when useful for understanding vectorization, numerical computing, and performance.

## Repository Structure

```text
ml-algorithms-from-scratch/
├── linear_regression.py
├── README.md
└── ...
```

As the project grows, each algorithm will have its own implementation and supporting experiments.

## Learning Philosophy

The objective isn't simply to reproduce the output of an ML library. It's to understand the processes that produce it.

For each algorithm, I aim to explore:

1. **Intuition:** What problem does the algorithm solve?
2. **Mathematics:** What equations and optimization methods does it use?
3. **Implementation:** How can it be built from the ground up?
4. **Experiments:** How do hyperparameters and data affect its behavior?
5. **Evaluation:** How does the implementation compare with established libraries?

## Long-Term Goal

Build a strong foundation in machine learning and deep learning by understanding algorithms at the mathematical and implementation levels, progressing toward neural networks, optimization, and the systems that make modern ML possible.

---

*Learning by implementing. Understanding by experimenting.*
