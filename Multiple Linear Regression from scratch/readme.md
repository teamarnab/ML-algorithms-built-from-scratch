# Multiple Linear Regression from Scratch

This project demonstrates the implementation of the Multiple Linear Regression algorithm from scratch using Python. Instead of relying on libraries like Scikit-learn, this project focuses on understanding and coding the underlying mechanics of the algorithm, including Ordinary Least Squares (OLS) for parameter estimation.

## Features

- Implementation of the Multiple Linear Regression algorithm without external libraries.
- Derivation of coefficients using the Ordinary Least Squares (OLS) method.
- Predictive model evaluation with metrics such as Mean Squared Error (MSE) and R-squared.
- A hands-on example showcasing the application of the regression model on sample datasets.

## Project Structure

```
├── multiple_linear_regression.py    # Python script for the implementation
├── README.md                       # Project documentation
```

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/teamarnab/ML-algorithms-built-from-scratch/tree/main/Multiple%20Linear%20Regression%20from%20scratch
   ```

2. Navigate to the project directory:
   ```bash
   cd multiple-linear-regression
   ```

3. (Optional) Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open the `multimulti_linear_regression_from_scratch.py` script to explore the implementation details.
2. Run the script:
   ```bash
   python multiple_linear_regression.py
   ```
3. Modify or replace the dummy dataset file to test the model with your own data.

## Example

The following example demonstrates how to use the implemented model on a dataset:

```python

# Example dataset
X = [[1, 2], [2, 3], [4, 5]]  # Independent variables
y = [2, 3, 5]                # Dependent variable

# Initialize and fit the model
model = Regression()
model.train_model(X, y)

# Make predictions
predictions = model.predict([[3, 4]])
print(f"Predictions: {predictions}")
```

## Metrics Implemented

- **R-squared**: To determine the proportion of variance explained by the model.

## How It Works

1. **Data Preprocessing**: The dataset is prepared, ensuring all independent variables are properly formatted.
2. **OLS Method**: The regression coefficients are calculated using the formula:
   \[
   \beta = (X^T X)^{-1} X^T y
   \]
   where \(X\) is the matrix of features and \(y\) is the target variable.
3. **Model Evaluation**: After fitting the model, predictions are compared against actual values using the implemented metrics.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Whether it's optimizing the code, adding new features, or improving the documentation, your input is welcome!


## Acknowledgments

- This project is inspired by the desire to understand the fundamentals of machine learning algorithms.
- Special thanks to the open-source Python community for making tools and libraries accessible.
