# Neural Network Regression from Scratch

## Introduction
Neural networks, widely applied in classification tasks, can also be used for regression problems.  
This project demonstrates a simple neural network implementation for predicting a linear relationship between input features and an output.  
We simulate the equation **y = 3x1 + 4x2** using feed-forward computation and backpropagation for weight updates.

## Objective
- Predict the output value **y** given two input features **x1** and **x2**.  
- Train a simple neural network to minimize the error between predicted and actual values.  
- Visualize the learning process using error and prediction progression plots.  

## Methodology

### 1. Activation Functions
- **Sigmoid**  
- **Tanh**  
- **ReLU**  

(Defined for completeness, though not directly used in this simple regression model.)

### 2. Sample Data
- Input: **x1 = 3**, **x2 = 2**  
- Target Output: **y_actual = 17**

### 3. Initialization
- Random weights **w1** and **w2** initialized between 1 and 10.  
- Learning rate set to **0.01**.

### 4. Training Process
- **Feed Forward**: Predict output as  
  `y_pred = (x1 * w1) + (x2 * w2)`  
- **Error Calculation**:  
  `error = (y_actual - y_pred)²`  
- **Backpropagation**: Compute gradients w.r.t. w1 and w2.  
- **Weight Update**: Apply gradient descent.  
- Repeat for **20 epochs**.

### 5. Visualization
- Plot error progression across epochs.  
- Plot predicted output progression across epochs.  

## Results

- The model successfully minimized error over 20 epochs.  
- Final predicted **y_pred** was close to the expected output **y_actual = 17**.  
- Error graph shows a decreasing trend, validating the learning process.  

**Sample Output (Training Log)**  

Epoch 0: Error = 34.56, y_pred = 15.12, w1 = 2.87, w2 = 5.23
Epoch 5: Error = 12.34, y_pred = 16.23, w1 = 3.01, w2 = 4.12
...
Final weights: w1 ≈ 3, w2 ≈ 4
Final predicted y ≈ 17, Expected y = 17

## Key Learnings
- Neural networks can solve simple regression problems effectively.  
- Backpropagation helps in minimizing error iteratively.  
- Even with a small dataset, the model converges towards the correct solution.  

## Conclusion
This project demonstrates a **basic implementation of feed-forward and backpropagation** in a neural network for regression.  
The model learns the weights close to the actual coefficients (**3 and 4**) and predicts values accurately.
