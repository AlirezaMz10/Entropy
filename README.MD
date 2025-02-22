# Entropy Calculation in Python

## Overview
This repository contains a Python implementation of entropy calculation for a given dataset. Entropy is a key concept in information theory and machine learning, particularly in decision tree algorithms. The script computes the entropy for different attributes of a dataset and helps in understanding the significance of each attribute in classification.

## Features
- Computes entropy for categorical and continuous variables
- Uses weighted average entropy to find the best split point
- Works with a NumPy array as input data
- Provides entropy calculations for multiple attributes

## Requirements
This script requires Python 3.x and the following libraries:

```bash
pip install numpy
```

## Usage
Clone the repository and run the script:

```bash
git clone https://github.com/AlirezaMz10/Entropy.git
cd Entropy
python entropy.py
```

## Code Explanation
The main functions in the script are:

### `calc_entropy(data)`
This function calculates entropy for a given dataset by splitting it based on unique values in the first column. It computes entropy using the formula:

$$ H(X) = - \sum p(x) \log_2 p(x) $$

### `calc_wighted_average(enp1, enp1_multiplier, enp2, enp2_multiplier)`
This function computes the weighted average entropy when splitting the dataset.

### Example Dataset
The dataset used is a NumPy array with four attributes:
- Column 0: Binary feature (e.g., Yes/No)
- Column 1: Binary feature (e.g., Yes/No)
- Column 2: Continuous feature (e.g., Age)
- Column 3: Target variable (Yes/No classification)

### Sample Output
The script prints the entropy values for different attributes and their impact on classification.

```python
print(calc_entropy(df[:, [0, -1]]))
print(calc_entropy(df[:, [1, -1]]))
print(calc_entropy(df[:, [2, -1]]))
```

## Author
[Your Name]

## License
This project is licensed under the MIT License.

