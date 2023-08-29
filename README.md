# Exploring Poisson Distributions with and without Truncation

In this code, we are exploring Poisson distributions with and without truncation using Python. We will generate random data points from Poisson distributions and fit Poisson probability mass functions to the data. Truncation involves setting values less than 1 to 1 in order to investigate the effects of truncation on the distribution.

## Importing Libraries

We start by importing the necessary libraries:
- `numpy` for numerical operations.
- `matplotlib.pyplot` for creating plots.
- `scipy.stats.poisson` for the Poisson distribution.
- `scipy.optimize.curve_fit` for fitting the Poisson probability mass function.

## Functions

### Truncated Poisson Function

The `truncated_poisson` function generates random data points from a Poisson distribution. If a `seed_value` is provided, it sets the random seed for reproducibility. The generated data is then truncated to have a minimum value of 1.

### Poisson Probability Mass Function Fit

The `poisson_fit` function calculates the Poisson probability mass function for a given set of data points and a lambda parameter.

### Plotting Function

The `plot_poisson_distribution` function takes data, color, alpha (transparency), and label as input. It creates a histogram of the data, fits a Poisson distribution using curve fitting, and plots the histogram and fitted curve on the same plot.

## Main Code

The main code starts by creating a figure with two subplots using `plt.figure` and `plt.subplot`.

### First Subplot

We set the mean degree (`mean_degree`), number of data points (`n`), and seed value for random number generation. Then, we generate two sets of data points: one with a random Poisson distribution and another with a truncated Poisson distribution. These data points are plotted using the `plot_poisson_distribution` function.

### Second Subplot

We repeat the process for a different mean degree, generating random and truncated Poisson data, and plotting them again.

Finally, we adjust the layout with `plt.tight_layout()` and display the plots using `plt.show()`.

This code demonstrates how to generate, visualize, and compare Poisson distributions with and without truncation using Python and relevant libraries.
