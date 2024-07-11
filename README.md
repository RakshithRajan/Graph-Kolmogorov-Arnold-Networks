# GKAN: Graph Kolmogorov-Arnold Networks

## Overview

This project re-implements the latest research paper on Kolmogorov-Arnold Networks (KANs) by **Ziming Liu, Yixuan Wang, Sachin Vaidya, Fabian Ruehle, James Halverson, Marin Soljačić, Thomas Y. Hou, and Max Tegmark**. Inspired by the Kolmogorov-Arnold representation theorem, KANs are proposed as alternatives to Multi-Layer Perceptrons (MLPs), featuring learnable activation functions on edges ("weights"). Notably, KANs replace all linear weights with univariate spline functions, demonstrating superior performance in accuracy and interpretability.

## Kolmogorov-Arnold Networks (KANs)

Kolmogorov-Arnold Networks (KANs) are inspired by the Kolmogorov-Arnold representation theorem, which states that any continuous multivariate function can be represented as a composition of a finite number of functions of fewer variables. In the context of neural networks, KANs extend this concept by using learnable activation functions on edges instead of fixed activation functions on nodes. This allows KANs to stack layers effectively and optimize network performance while maintaining interpretability.

The formula for a single layer in KANs is represented as follows:

\[ y = \sigma(\sum_{j=1}^{d} w_j \cdot \phi_j(x)) \]

where \( \sigma \) is the activation function, \( w_j \) are the learnable weights, \( \phi_j \) are spline functions parameterized on edges, and \( x \) is the input data.

## Comparison with MLPs

Multi-Layer Perceptrons (MLPs) have traditionally been the standard neural network architecture, using fixed activation functions on nodes. While MLPs are effective, KANs introduce several advancements:

- **Learnable Activation Functions:** KANs use spline-based activation functions on edges, offering flexibility and enhancing model interpretability.
- **Stackability:** KANs allow layers to be stacked effectively, optimizing model performance across various tasks.
- **Performance:** Empirical evidence suggests that KANs can achieve comparable or superior accuracy to MLPs, particularly in tasks such as data fitting and solving partial differential equations (PDEs) on graph-structured data.
- **Interpretability:** KANs are intuitively visualized and facilitate interaction with users, aiding in the exploration and discovery of mathematical and physical laws in datasets.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/RakshithRajan/Graph-Kolmogorov-Arnold-Networks.git
   cd repository
