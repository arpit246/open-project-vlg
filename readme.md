# Hyperparameter Optimization for RandomForest Classifier

This project aims to optimize the hyperparameters of a RandomForest Classifier using a custom approach based on Kernel Density Estimation (KDE) and quantile segmentation.

## Table of Contents
- [Data Preperation](#project-description)
- [Objective function creation](#installation)
- [Search Space Formation](#usage)
  - [Sampling Initial trials ](#example)
- [HPO teachnique](#visualization)
- [Graphs Related](#results)
- [License](#license)

## Project Description
The goal of this project is to find the best hyperparameters for a RandomForest Classifier to maximize its accuracy. The optimization process involves:
1. Sampling hyperparameters from a predefined search space.
2. Evaluating these samples using cross-validation.
3. Using Kernel Density Estimation to model the distributions of good and bad hyperparameter sets.
4. Iteratively selecting new hyperparameter sets to test based on these distributions.

## Installation
To run this project, you'll need Python 3.x and several Python libraries. You can install the required libraries using the following command:

```bash
pip install numpy pandas scikit-learn seaborn hyperopt
