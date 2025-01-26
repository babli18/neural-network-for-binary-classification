 **Exploring Neural Networks for Binary Classification: XOR and Beyond**
==========================================================================

## **Overview**
This case-study demonstrates the use of neural networks for solving binary classification tasks, from the classic XOR problem to real-world datasets (exclipse and hexagon) with unique patterns. The study focuses on exploring network architectures, training techniques, and decision boundary visualizations to derive key insights.


## **Contents**
- [Objectives](#objectives)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Results and Insights](#results-and-insights)
- [Conclusion](#conclusion)


## **Objectives**
1. **XOR Classification**:
   - Address the challenge of classifying non-linearly separable XOR data.
   - Explore the minimal neural network architecture needed for accurate classification.
2. **Real-World Data Classification**:
   - Classify binary-labeled data from two custom datasets ("ellipse" and "hexagonal" patterns).
   - Determine optimal network architectures for these datasets.


## **Data Description**
- **XOR Data**:
  - Input: Four binary combinations \([0,0], [0,1], [1,0], [1,1]\).
  - Labels: \(0\) or \(1\), representing an XOR logic gate.

- **Custom Datasets**:
  - `FeedForward_Data_ellipse.csv`: Two-dimensional binary-labeled data forming an elliptical distribution.
  - `FeedForward_Data_hexa.csv`: Two-dimensional binary-labeled data forming a hexagonal distribution.


## **Methodology**
- **Data Preprocessing**:
  - Data split into training, validation, and test sets.
  - Conversion of data into PyTorch tensors for efficient training.
- **Model Architectures**:
  - Customizable feedforward neural networks with varying numbers of hidden layers and neurons.
- **Training Techniques**:
  - Loss functions: Mean Squared Error (MSE) and Binary Cross-Entropy.
  - Optimization using gradient descent with early stopping.


## **Results and Insights**
### XOR Classification:
- **Smallest network achieving 100% accuracy**:
  - Architecture: 1 hidden layer with 2 neurons.

### Real-World Data Classification:
#### **"Ellipse" Dataset**:
- **Best Loss**: 0.1944
- **Best Accuracy**: 90.34%
- **Optimal Architecture**: 4 hidden layers with [256, 512, 256, 128] neurons.

#### **"Hexagonal" Dataset**:
- **Best Loss**: 0.0616
- **Best Accuracy**: 96.90%
- **Optimal Architecture**: Same as "Ellipse."

### Visualizations:
- Decision boundary plots illustrate how the models separate binary classes for each dataset.


## **Conclusion**
- Neural networks, even with basic architectures, can solve challenging binary classification problems effectively.
- Experimenting with architecture depth and capacity is key to optimizing performance.
- Visualizations enhance interpretability and provide actionable insights into model behavior.

