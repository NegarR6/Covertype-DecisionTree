# 🌳 Decision Tree Classifier: Implementation From Scratch

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![ML](https://img.shields.io/badge/Focus-Machine%20Learning-orange.svg)]()
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An advanced implementation of the Decision Tree algorithm from the ground up, designed to solve complex multi-class classification problems. This project demonstrates the core mechanics of machine learning without relying on high-level library abstractions for the model itself.

##  Project Overview
This repository contains a pure Python implementation of a Decision Tree, evaluated on the **UCI Covertype Dataset**. The goal is to predict forest cover types based on 54 cartographic variables (elevation, slope, soil types, etc.).

### Key Technical Features
* **Mathematical Core:** Implemented both **Information Gain (Entropy)** and **Gini Impurity** as splitting criteria.
* **Data Pipeline:** Custom **Quartile Binning** strategy to transform continuous environmental data into meaningful categorical buckets.
* **Overfitting Control:** A robust **Post-Pruning** algorithm that uses a validation set to trim the tree for better generalization.
* **Vivid Analytics:** * Structural visualization of the tree using `networkx`.
    * Comprehensive performance metrics including Confusion Matrices and Per-Class accuracy.
    * Feature Importance analysis based on split frequency.

##  Architecture & Implementation
Unlike standard library calls, this implementation builds the tree recursively:
1.  **Splitting:** Exhaustive search for the best feature/value pair that maximizes Information Gain.
2.  **Pruning:** Bottom-up traversal to compare accuracy before and after removing nodes, ensuring the simplest effective model.
3.  **Visualization:** Dynamic mapping of the tree nodes into a directed graph for interpretability.

##  Getting Started

### Prerequisites
- Python 3.x
- Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, NetworkX

### Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/NegarR6/Covertype-DecisionTree.git](https://github.com/NegarR6/Covertype-DecisionTree.git)
   
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   
3. Run the analysis:
   ```bash
   python final.py

### License
This project is licensed under the MIT License - see the LICENSE file for details.

Developed by Negar Rezaei | GitHub @NegarR6
