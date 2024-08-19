# Day 1 Machine Learning

Welcome to the Day 1 Machine Learning repository! This repository contains various resources and examples to kickstart your journey into machine learning. 

## Overview of Pandas Statistical Operations

Pandas is a powerful library for data manipulation and analysis in Python. This README provides an overview of common statistical operations available in Pandas that are essential for data analysis and preprocessing in machine learning projects.

### Basic Statistics

1. **Descriptive Statistics**

   - **`DataFrame.describe()`**: Provides summary statistics for numerical columns, including count, mean, standard deviation, min, 25th percentile, median (50th percentile), 75th percentile, and max.
   - **`Series.describe()`**: Provides summary statistics for a single Series.

2. **Mean and Median**

   - **`DataFrame.mean()`**: Returns the mean of the values for each column.
   - **`Series.mean()`**: Returns the mean of the values in the Series.
   - **`DataFrame.median()`**: Returns the median of the values for each column.
   - **`Series.median()`**: Returns the median of the values in the Series.

3. **Standard Deviation and Variance**

   - **`DataFrame.std()`**: Returns the standard deviation of the values for each column.
   - **`Series.std()`**: Returns the standard deviation of the values in the Series.
   - **`DataFrame.var()`**: Returns the variance of the values for each column.
   - **`Series.var()`**: Returns the variance of the values in the Series.

4. **Min and Max**

   - **`DataFrame.min()`**: Returns the minimum value of each column.
   - **`Series.min()`**: Returns the minimum value in the Series.
   - **`DataFrame.max()`**: Returns the maximum value of each column.
   - **`Series.max()`**: Returns the maximum value in the Series.

5. **Percentiles and Quantiles**

   - **`DataFrame.quantile(q)`**: Returns the quantile(s) of the values for each column. `q` can be a single value (e.g., 0.5 for the median) or a list of values.
   - **`Series.quantile(q)`**: Returns the quantile(s) of the values in the Series.

### Correlation and Covariance

1. **Correlation**

   - **`DataFrame.corr()`**: Computes pairwise correlation of columns, excluding NA/null values. By default, it uses Pearson correlation, but methods like Kendall or Spearman can also be specified.
   - **`Series.corr(other, method='pearson')`**: Computes the correlation between the Series and another Series or DataFrame.

2. **Covariance**

   - **`DataFrame.cov()`**: Computes pairwise covariance of columns, excluding NA/null values.
   - **`Series.cov(other)`**: Computes the covariance between the Series and another Series or DataFrame.

### Aggregation Operations

1. **Sum, Count, and Product**

   - **`DataFrame.sum()`**: Returns the sum of the values for each column.
   - **`Series.sum()`**: Returns the sum of the values in the Series.
   - **`DataFrame.count()`**: Returns the count of non-NA/null values for each column.
   - **`Series.count()`**: Returns the count of non-NA/null values in the Series.
   - **`DataFrame.prod()`**: Returns the product of the values for each column.
   - **`Series.prod()`**: Returns the product of the values in the Series.

2. **Cumulative Statistics**

   - **`DataFrame.cumsum()`**: Returns the cumulative sum of the values for each column.
   - **`Series.cumsum()`**: Returns the cumulative sum of the values in the Series.
   - **`DataFrame.cumprod()`**: Returns the cumulative product of the values for each column.
   - **`Series.cumprod()`**: Returns the cumulative product of the values in the Series.

### Additional Operations

1. **Skewness and Kurtosis**

   - **`DataFrame.skew()`**: Returns the skewness (asymmetry of the distribution) for each column.
   - **`Series.skew()`**: Returns the skewness of the values in the Series.
   - **`DataFrame.kurt()`**: Returns the kurtosis (tailedness of the distribution) for each column.
   - **`Series.kurt()`**: Returns the kurtosis of the values in the Series.

2. **Mode**

   - **`DataFrame.mode()`**: Returns the mode(s) of the values for each column.
   - **`Series.mode()`**: Returns the mode(s) of the values in the Series.

3. **Correlation Matrix**

   - **`DataFrame.corrwith(other)`**: Computes the correlation of the DataFrame with another DataFrame or Series.

## Getting Started

To start using these Pandas operations, ensure you have Pandas installed in your environment:

```bash
pip install pandas


import pandas as pd

# Example usage
df = pd.DataFrame({
    'A': [1, 2, 3, 4, 5],
    'B': [5, 4, 3, 2, 1]
})

print(df.describe())
print(df.mean())
print(df.corr())
