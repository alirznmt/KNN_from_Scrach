# k-NN Implementation for Employee Data Classification

## Overview
This project implements a k-nearest neighbors (k-NN) classifier to predict employee attrition using the Employee Data Classification dataset. The project includes cross-validation to select the optimal value of k and optimizations to improve computational efficiency.

## Dataset
The Employee Data Classification dataset has been used. The dataset is available here.. The dataset comprises 7 features and a label feature named "LeaveOrNot".

## Project Steps
1. **Data Loading**: Load the dataset into Python.
2. **Data Visualization**: Plot histograms or bar charts to represent the dataset containing labels and features.
3. **Data Splitting**:
   - Split the data into training (80%) and test (20%) sets.
4. **1-Nearest Neighbor Classifier**:
   - Train a 1-nearest neighbor classifier using the training data.
   - Predict the labels on the test data and calculate the test error.
5. **Optimal k Selection**:
   - Train the k-NN classifier for k ∈ {1, 3, 5, 7, 9, 11, 13}.
   - Compute the test error for each k.
   - Choose the optimal k based on the test errors.
   - Compute the error rate of the classifier for the optimal k on the validation set.

### Computational Cost Optimization
1. **Priority Queue Heap Data Structure**:
   - Initialize a heap with k points from the training dataset based on their distances to the query point.
   - Iterate through the dataset, maintaining the k nearest neighbors in the heap.
   - Rewrite the k-NN using the heap data structure and compare its running time performance to the ordinary k-NN with k = 5.
2. **k-d Tree Data Structure**:
   - Use a k-d tree data structure to improve the efficiency of the k-NN implementation.
   - Compare the running time of the k-d tree implementation to the heap and ordinary k-NN with k = 5.

### Optional Enhancement
1. **Dimensionality Reduction**:
   - Apply dimension reduction techniques to the dataset.
   - Implement k-NN on the reduced dataset.
   - Compare the running time of k-NN on the original dataset versus the reduced dataset with k = 5.

## Requirements
- Python 3.x
- Libraries: pandas, numpy, matplotlib, scikit-learn, heapq

## How to Run
1. Clone the repository.
2. Install the required libraries.
3. Run the Jupyter notebook or Python scripts provided.

## Results
- The optimal
