# Federated Learning with Homomorphic Encryption Optimized Neural Networks

## Overview

This framework enables federated learning with privacy-preserving and secure neural network training. It leverages homomorphic encryption to allow multiple clients to collaborate and enhance the accuracy of neural network models without sharing their raw data.

This README provides an overview of the Python library, including its components, usage, and examples. Additionally, it includes information on the code example provided in the repository.

## Table of Contents

- [Introduction](#introduction)
- [Key Features](#key-features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Code Examples](#code-examples)
- [License](#license)
- [Authors](#authors)

## Introduction

The framework provides a federated learning solution for both classification and regression tasks. It consists of two main components:

1. **Client**: Clients are responsible for training models locally on their data. They support different activation functions (e.g., sigmoid, ReLU, linear) and can be configured to use homomorphic encryption for privacy.

2. **Coordinator**: The coordinator aggregates models from multiple clients and computes an optimized global model using federated learning. It supports L2 regularization and can use homomorphic encryption to protect the model's privacy.

The library is highly customizable and can be adapted to various use cases, including classification and regression tasks. It also allows you to choose whether to use encryption and sparse matrices for optimization.

## Key Features

- **Privacy-Preserving Learning**: Clients can use homomorphic encryption to protect their data while contributing to model training.

- **Customizable Activation Functions**: Clients can choose between logistic sigmoid, ReLU, and linear activation functions for their models.

- **Sparse Matrices**: Supports the use of sparse matrices for improved performance on large datasets.

- **Federated Learning**: Enables federated learning, where multiple clients collaborate to create a global model without sharing their data directly.

- **Regularization**: The coordinator supports L2 regularization to improve model generalization.

## Installation

To install the framework, follow these steps:

1. Clone the repository from GitHub.
2. Install the required dependencies using pip or conda.
3. Start using the library in your projects.

## Usage

Detailed usage instructions for both the client and coordinator components are available in the code's documentation. Below is a high-level overview:

### Client

- Create a client with activation function and encryption options.
- Fit the client's model with local data.
- Provide the aggregated models to the coordinator for federated learning.
- Use the model to make predictions.

### Coordinator

- Create a coordinator with activation function and regularization options.
- Aggregate models from multiple clients using federated learning.
- Provide the aggregated global model to clients.
- Clients can use the received global model for predictions.

## Code Examples

### Carbon Nanotubes Regression

The repository includes a code example for using the framework to perform federated regression on a Carbon Nanotubes dataset. It demonstrates how to train models across multiple clients, aggregate them, and evaluate their performance.

### Dry Bean Classification

Another code example in the repository focuses on Dry Bean classification, showing how to use the framework for federated classification tasks.



