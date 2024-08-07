# Probability Examples in Python

This repository provides an introduction to probability with real-world examples implemented in Python. Probability is a measure of the likelihood that an event will occur, expressed as a number between 0 and 1. A probability of 0 means the event will not occur, and a probability of 1 means the event will certainly occur.

## Table of Contents

1. [Introduction to Probability](#introduction-to-probability)
2. [Examples](#examples)
    - [Coin Toss](#coin-toss)
    - [Weather Forecasting](#weather-forecasting)
    - [Quality Control in Manufacturing](#quality-control-in-manufacturing)
    - [Stock Market Simulation](#stock-market-simulation)
    - [Credit Scoring](#credit-scoring)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction to Probability

Probability is used in various fields such as statistics, mathematics, finance, gambling, science, and engineering. It helps to predict the likelihood of different outcomes in uncertain situations.

The probability of an event \( A \) is given by:

\[ P(A) = \frac{\text{Number of favorable outcomes}}{\text{Total number of possible outcomes}} \]

## Examples

### Coin Toss

A simple example of probability is the coin toss. The probability of getting heads or tails in a fair coin toss is 0.5.

```python
import numpy as np

# Simulate tossing a coin 10,000 times
num_tosses = 10000
tosses = np.random.choice(['Heads', 'Tails'], size=num_tosses)

# Count the number of heads and tails
heads_count = np.sum(tosses == 'Heads')
tails_count = np.sum(tosses == 'Tails')

# Calculate probabilities
prob_heads = heads_count / num_tosses
prob_tails = tails_count / num_tosses

print(f"Probability of Heads: {prob_heads:.4f}")
print(f"Probability of Tails: {prob_tails:.4f}")