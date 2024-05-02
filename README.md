# DATA-SCIENCE-DIARY
My personal endeavors and learning experiences in the field of data science.

# April 2024
29/04/2024 - 30/04/2024

LINEAR REGRSIION
  - An exploration of the significance of the Gradient Descent method and its distinctions from the Least Squares method.
    - LEAST SQUARE METHOD
      - To minimise the loss function $\sum (y - predicted \ y )^2$
      - Utilize the matrix equation $(X^TX)^{-1}(X^TY)$ (normal equation ) for calculating the coefficients of regression.
      - The LinearRegression model in scikit-learn computes the pseudo-inverse of the matrix using Singular Value Decomposition (SVD) to manage scenarios where the matrix is not invertible.
        
    - GRADIENT DESCENT
        - The computational efficiency of both the Normal Equation and Singular Value Decomposition (SVD) methods tends to diminish significantly as the number of features in a dataset increases (e.g., reaching 100,000). In such cases, Gradient Descent emerges as a preferred alternative due to its scalability and efficiency in handling large-dimensional data.

# May 2024
1/05/24

LOGISTIC REGRESSIONN (STATISTICAL MODELING) 
  - Logistic regression is used to model categorical variables 𝑦 that take two values and $y$ depends on the variable $x$.
  - For example, the passing or failing of students may depend on the number of hours they study.
  - If we consider 𝑝 as the probability of success, then it is dependent on the value of 𝑥. Therefore, we denote it as 𝑝(𝑥) to reflect this dependency.
  - Logit function
    $$p(x) = \frac{ e^{\beta_0 + \beta_1 x}}{1 + e^{\beta_0 + \beta_1 x}}$$

  - Logistic regression means assuming that $p(x)$ is related to x by the logit function

  - It can be shown that $$\frac{p(x)}{1 - p(x)} = e^{\beta_0 + \beta_1 x}$$
  - $\frac{p(x)}{1 - p(x)}$ is called as $odds$
  - If we take $ln$ on both sides of above equation, it becomes $ln(\frac{p(x)}{1 - p(x)}) = \beta_0 + \beta_1 x $
  - Coefficients $\beta_0$ and $\beta_1$ is calculated using maximum likelihood estimation.
  - We can make use of Logit() function from statsmodels.api for statistical analysis with logistic regression. 
    
    

