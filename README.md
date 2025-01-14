# Logistic Regression and EM Algorithm

This project includes two main parts: **Logistic Regression** for binary classification and the **Expectation-Maximization (EM) Algorithm** for clustering MNIST images into ten groups. Both parts involve custom implementation of algorithms with manual optimization techniques.

---

## Part 1: Logistic Regression

### Features
1. **Data Generation**:
   - Generate two datasets (`D1` and `D2`) using Gaussian distributions with specified means and variances for `x` and `y` coordinates.
2. **Optimization Methods**:
   - **Newton's Method**: Used for faster convergence unless the Hessian is singular.
   - **Steepest Gradient Descent**: Fallback method when Newton's Method is not feasible.
3. **Performance Metrics**:
   - Computes confusion matrix, sensitivity, and specificity for training data.
4. **Visualization**:
   - Plots ground truth and predicted classification results.

### Usage
1. **Inputs**:
   - Number of data points (`N`).
   - Means and variances for `D1` and `D2` in the format `mx1, vx1, my1, vy1, mx2, vx2, my2, vy2`.
2. **Outputs**:
   - Confusion matrix.
   - Sensitivity and specificity metrics.
   - Visual plots for ground truth and predictions.

---

## Part 2: Expectation-Maximization (EM) Algorithm

### Features
1. **Data Preprocessing**:
   - Bins MNIST grayscale pixel values into two levels (binary representation).
   - Treats each pixel as a Bernoulli random variable.
2. **EM Algorithm**:
   - Clusters images into ten groups using an iterative EM approach.
   - Determines convergence based on a reasonable threshold or maximum iteration rule.
3. **Performance Metrics**:
   - Outputs confusion matrix, sensitivity, and specificity for clustering results.
   - Assigns labels to clusters post hoc for evaluation purposes.
4. **Visualization**:
   - Binary visualizations of the classifier's understanding of each digit.

### Usage
1. **Inputs**:
   - MNIST training data and labels.
2. **Outputs**:
   - Confusion matrix for each digit.
   - Sensitivity and specificity of clustering.
   - Binary representations of digits learned by the model.

---

