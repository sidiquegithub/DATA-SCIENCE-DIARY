# DATA-SCIENCE-DIARY
My personal endeavors and learning experiences in the field of data science.

# April 2024
29/04/2024

LINEAR REGRSIION
  - An exploration of the significance of the Gradient Descent method and its distinctions from the Least Squares method.
    - LEAST SQUARE METHOD
      - To minimise the loss function $\sum (y - predicted \ y )^2$
      - Utilize the matrix equation $(X^TX)^{-1}(X^TY)$ (normal equation ) for calculating the coefficients of regression.
      - The LinearRegression model in scikit-learn computes the pseudo-inverse of the matrix using Singular Value Decomposition (SVD) to manage scenarios where the matrix is not invertible.
        
    - GRADIENT DESCENT
        - The computational efficiency of both the Normal Equation and Singular Value Decomposition (SVD) methods tends to diminish significantly as the number of features in a dataset increases (e.g., reaching 100,000). In such cases, Gradient Descent emerges as a preferred alternative due to its scalability and efficiency in handling large-dimensional data.


