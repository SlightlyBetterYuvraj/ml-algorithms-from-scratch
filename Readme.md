# Linear Regression From Scratch

A pure Python implementation of **multivariable linear regression using batch gradient descent**, built from scratch to understand the mathematics and mechanics behind machine learning algorithms.

No scikit-learn. No NumPy. Just Python, mathematics, and gradient descent.

## What I Built

Started with single-feature linear regression and extended it to support multiple input features dynamically.

The model learns a weight for each feature and a bias to minimize the Mean Squared Error (MSE) between its predictions and the actual targets.

### Model

For multiple features, the prediction is:

\[
\hat{y} = w_1x_1 + w_2x_2 + \cdots + w_dx_d + b
\]

Where:
- \(x_j\) — input feature
- \(w_j\) — learned weight for that feature
- \(b\) — bias
- \(\hat{y}\) — predicted output

## Concepts Implemented

- [x] Single-feature linear regression
- [x] Multivariable linear regression
- [x] Weight and bias initialization
- [x] Mean Squared Error (MSE)
- [x] Gradient calculation for each feature
- [x] Batch gradient descent
- [x] Iterative parameter updates
- [x] Dynamic support for multiple input features

## How Training Works

1. Initialize all weights and the bias to zero.
2. Calculate predictions using the current parameters.
3. Calculate prediction errors.
4. Accumulate gradients for each weight and the bias.
5. Update the parameters using gradient descent.
6. Repeat for the specified number of epochs.

### Loss Function

Mean Squared Error measures the average squared prediction error:

\[
MSE = \frac{1}{n}\sum_{i=1}^{n}(\hat{y}_i-y_i)^2
\]

### Gradient Descent

The parameters are updated using:

\[
w_j \leftarrow w_j-\alpha\frac{\partial MSE}{\partial w_j}
\]

\[
b \leftarrow b-\alpha\frac{\partial MSE}{\partial b}
\]

Where \(\alpha\) is the learning rate.

## Example Experiment

I tested the model with **5 features and 20 training examples**. The target values were generated using a known linear equation:

\[
y=4x_1-2x_2+3x_3+0.5x_4+6x_5+10
\]

This allowed me to compare the parameters learned by gradient descent against the known parameters.

### Results

| Parameter | Expected | Learned |
|---|---:|---:|
| Weight 1 | 4.0 | 4.028 |
| Weight 2 | -2.0 | -1.958 |
| Weight 3 | 3.0 | 3.038 |
| Weight 4 | 0.5 | 0.546 |
| Weight 5 | 6.0 | 6.030 |
| Bias | 10.0 | 9.370 |
| Training MSE | 0.0 | 0.00544 |

*Experiment settings: 10,000 epochs and a learning rate of 0.01.*

The model learned parameters close to the known values and achieved a low training MSE.

## Tech Stack

- **Language:** Python
- **Dependencies:** None
- **Approach:** Pure Python implementation

## Running the Project

1. Clone the repository.
2. Open the Python script containing the implementation.
3. Run it with Python 3.

```bash
python linear_regression.py
```

Replace `linear_regression.py` with the actual filename if yours differs.

## What I Learned

This project helped me understand:

- How weights and bias control a linear model's predictions.
- How loss functions measure prediction error.
- How gradients determine the direction and magnitude of parameter updates.
- Why gradient accumulation must happen before updating parameters in batch gradient descent.
- How the same algorithm can support different numbers of features without rewriting its core logic.

The goal wasn't just to use an existing machine learning library. It was to understand what happens underneath the API.

## What's Next?

- [ ] Implement logistic regression from scratch.
- [ ] Implement K-Nearest Neighbors.
- [ ] Build a decision tree classifier.
- [ ] Implement a small neural network and backpropagation.
- [ ] Compare custom implementations against scikit-learn.

---
**Learning machine learning by rebuilding it from the ground up.**