# utils: Data 301 Utility Functions

A collection of reusable Python utilities developed for data analysis, visualization, and common data science tasks in Data 301.

## Overview

This package provides convenient functions and utilities to support data analysis workflows, particularly for the Data 301 course. It includes helpers for data loading, preprocessing, visualization, and statistical analysis, enabling faster development and cleaner code.

## Features

- **Data Loading & Processing**: Streamlined data import and cleaning
- **Statistical Functions**: Common statistical calculations and testing
- **Visualization Helpers**: Pre-configured plotting functions for common scenarios
- **Data Validation**: Input validation and data quality checks
- **Convenience Functions**: Common operations wrapped for ease of use
- **Transformations**: Data transformation utilities for preparation and feature engineering

## Installation

```bash
# Install from requirements
pip install -r requirements.txt
```

Or install from the repository:

```bash
git clone https://github.com/eren-onat/utils.git
cd utils
pip install -e .
```

Or add to your Python path:

```python
import os
import sys
PROJECT_ROOT = os.path.abspath(os.path.join(os.getcwd(), os.pardir))
if PROJECT_ROOT not in sys.path:
    sys.path.append(PROJECT_ROOT)

from utils.transforms import *
```

## Usage Example

```python
from utils import load_data, plot_distribution, clean_data

# Load and clean data
df = load_data('data.csv')
df = clean_data(df)

# Quick visualization
plot_distribution(df['column_name'])
```

## Available Utilities

### Data Functions
- Data loading and caching
- Missing value handling
- Outlier detection and treatment
- Type inference and validation
- Data transformation and feature engineering

### Analysis Functions
- Summary statistics
- Correlation analysis
- Statistical tests
- Hypothesis testing helpers
- Distribution analysis

### Visualization Functions
- Distribution plots
- Correlation matrices
- Time series visualization
- Comparison plots
- Heatmaps and scatter plots

## Documentation

Detailed documentation is available in the source code docstrings. Use `help()` or `?` in Jupyter notebooks for function documentation.

```python
from utils import load_data
help(load_data)  # Display detailed function documentation
```

## Contributing

This is a course utility package. Feel free to fork and adapt for your own projects.

## Technologies

- **Python 3.8+**
- **pandas**: Data manipulation
- **NumPy**: Numerical computing
- **Matplotlib/Seaborn**: Visualization
- **SciPy**: Statistical functions

## License

This utility package is provided for educational purposes.

## Author

Eren Onat - [GitHub](https://github.com/eren-onat)

## Questions?

Refer to the docstrings in the source code or check the course materials for more information.
