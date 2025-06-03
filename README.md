# Linear Regression Using Gradient Descent

A from-scratch implementation of simple linear regression using manual gradient descent — no sklearn or built-in optimizers used.

---

## What I Did

- Loaded numeric (x, y) data and split into train/test sets
- Shuffled the data using df.sample(frac = 1), because using libraries is a sin, absolutely EVERYTHING has to manual :).
- Initialized slope and intercept
- Iteratively updated parameters using gradient descent
- Stopped when error dropped below a defined threshold

---

## Results

- Converged in ~43,000 steps => MSE was below 0.5.
- Final learned model:    y = 0.96x + 3.16
- Visualized predictions vs actual data points on the test set
- Visually this plot is VERY slightly off.
- The initial conditions in this notebook [5,10] are pretty far from the actual final coefficients. I kept it as it is just to see how many iterations it would take to converge from such... unforgiving, for the lack of a better word, initial conditions. 
- We get MUCH closer plots for the same initial conditions, when allowed to run close to 50000 iterations, but my laptop expressed great anguish the last time I did that.

---

## Takeaway

Though small in scale, this project was crucial for building hands-on understanding of:
- Loss functions
- Gradients
- Model convergence

It laid the foundation for more advanced model tuning in later projects.
