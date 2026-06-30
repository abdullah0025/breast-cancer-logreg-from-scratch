# breast-cancer-logreg-from-scratch
Binary classifier (malignant vs benign) built from scratch with NumPy — sigmoid, cost function, and gradient descent implemented manually, no sklearn model used

## What this does
- Loads the sklearn breast cancer dataset (no pandas needed)
- Splits into train / val / test (70/15/15)
- Scales features with z-score normalization
- Logistic regression from scratch — sigmoid, cost function, gradient descent, no `sklearn.linear_model` used

## Results
- Validation accuracy: 98%

## What I learned
- Feature scaling matters a lot once you're hand-rolling gradient descent — unscaled features made the cost diverge
- Numerically stable sigmoid (avoiding exp overflow) and clipping before log() to handle edge cases
