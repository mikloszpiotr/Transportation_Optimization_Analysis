# Transportation Optimization with Machine Learning

This project demonstrates how to optimize supply chain logistics by determining the ideal locations for Distribution Centers (DCs) using Machine Learning.

## Objective
The goal is to minimize transportation costs and improve efficiency by grouping customers into optimal clusters and assigning them to the nearest Distribution Center. We use **K-Means Clustering**, an unsupervised machine learning algorithm, to solve this facility location problem.

## Features
- **Synthetic Data Generation**: Simulates a dataset of 200 customers located across the US East Coast with varying demand.
- **ML Optimization**: Uses **K-Means Clustering** to:
  - Group customers into 5 distinct regions.
  - Calculate the geometric center (centroid) of each region to identify the optimal location for a DC.
- **Interactive Visualization**: Generates a rich map using `folium` to visualize:
  - **Distribution Centers**: Marked with black stars.
  - **Customers**: Color-coded dots based on their assigned cluster.
  - **Routes**: Lines connecting each customer to their serving DC.

## Getting Started

### Prerequisites
Ensure you have Python installed along with the valid dependencies.

### Installation
1. Navigate to the project directory:
   ```bash
   cd transportation_optimization
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook transportation_optimization.ipynb
   ```
2. Run all cells in the notebook to generate the data, perform the optimization, and view the interactive map.

## Dependencies
- `pandas`: Data manipulation
- `numpy`: Numerical operations
- `scikit-learn`: K-Means clustering algorithm
- `folium`: Map visualization
- `matplotlib` & `seaborn`: Plotting utilities
