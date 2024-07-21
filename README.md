# Smart Beta Portfolio Construction and Portfolio Optimization

Python program that creates  a smart beta portfolio and also generates a portfolio optimiation strategy.

The beta portfolio is constructed using the dividend yields to select portfolio weights.  Index weights are first constrcted based on a dollar volume average.  The two portfolios are then created using the derived weights with the index portfolio acting as a benchmark.  The tracking error is then calculated to compare the results of the beta and benchmark strategies.

An optimal portfolio is then created with the objective of minimizing the portfolio return variance as well as the distance between the vector of weights in the portfolio and the market cap weighted benchmark index.  The cvxpy package is used to perform a convex optimization strategy based on this objective.  The function is generalized to allow for a scalar factor to specify the importance of the distance in the portfolio weights.  Another strategy is develop to allow the portfolio weights to be balanced over time with consideration for determining the cost of rebalancing as well.

## Getting Started

The project_3_starter.ipynb notebook was modified in VS Code and uses the Python 3.12.3 library.  A requirements.txt file is included.  Libraries can be installed by installing the contents of this file or by executing the first line of the notebook.
