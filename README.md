# MyGaussian_Distribution_Package

## Overview

**MyGaussian_Distribution_Package** is a Python package that provides classes for working with probability distributions. The package currently supports both general probability distributions and Gaussian (normal) distributions. It allows users to calculate basic statistics, such as the mean and standard deviation, and visualize data with histograms and probability density functions.

## Features

- General `Distribution` class for managing probability distributions.
- `Gaussian` class, which extends the `Distribution` class to include:
  - Calculation of mean and standard deviation.
  - Visualization of histograms and probability density functions.
  - Ability to add two Gaussian distributions together.
- Read data from text files and perform statistical analysis.

## Installation

To install the package locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/kwoba98/MyGaussian_Distribution_Package.git
    ```

2. Navigate to the project directory:

    ```bash
    cd Mydistributions
    ```

3. Install the package locally:

    ```bash
    pip install .
    ```

### Requirements

Make sure to have the following dependencies installed (these will be installed automatically with the package):

- `matplotlib`

## Usage

Once installed, you can import and use the classes in your Python code as follows:

```python
from Mydistributions import Gaussian, Distribution

# Create a Gaussian distribution with mean=5 and standard deviation=2
gaussian = Gaussian(mu=5, sigma=2)

# Calculate the mean and standard deviation
gaussian.calculate_mean()
gaussian.calculate_stdev()

# Read data from a file
gaussian.read_data_file('data.txt')

# Plot a histogram of the data and the probability density function
gaussian.plot_histogram_pdf()

# Create a general distribution
dist = Distribution()
dist.read_data_file('data.txt')
