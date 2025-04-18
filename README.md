# Hacker Stats:

Welcome to **Hacker Stats**, where we dive into the fascinating world of random walks, probabilities, and statistics. Inspired by the spirit of friendly betting and data-driven decision-making, this project simulates a game where a player challenges their friend to reach a specific step in a building. The goal? Use **hacker stats** to estimate the likelihood of success and uncover insights through data and visualization.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Game Scenario](#game-scenario)
3. [Hacker Stats and Random Walk](#hacker-stats-and-random-walk)
4. [Features](#features)
5. [Setup](#setup)
6. [How to Run](#how-to-run)
7. [Outputs](#outputs)
   - [Dynamic Visualization](#dynamic-visualization)
   - [Distribution Plot and Statistical Analysis](#distribution-plot-and-statistical-analysis)
8. [References](#references)

---

## Introduction

The **Random Walk Challenge** is a fun and engaging way to explore the power of probabilities and data simulation. This project simulates a friendly competition where one player bets they can reach a specific step in a building within a set number of dice rolls. Using the principles of **hacker stats**, we simulate thousands of games, analyze the outcomes, and visualize the data to determine the likelihood of winning.

---

## Game Scenario

Imagine you're climbing a building with your friend, and you make a bet: Can you reach step 60 (or any target step) within 100 dice rolls? The rules of the game are simple:

1. **Roll a 6-sided die**:
   - Roll **1 or 2**: Move down one step (but not below step 0).
   - Roll **3, 4, or 5**: Move up one step.
   - Roll **6**: Roll again and move up the resulting number of steps.
   - Should not go below step 0.

2. **Clumsiness Factor**:
   - With a 0.1% chance, you might fall back to step 0 after any move.

3. **Winning the Bet**:
   - To win, you must reach or exceed the **target step** (e.g., step 60) within 100 rolls.

4. **Simulate to Win**:
   - To determine the probability of success, simulate this game thousands of times and analyze the results.

---

## Hacker Stats and Random Walk

**Hacker stats** refers to the use of simulation and computational methods to solve complex statistical problems. Instead of relying solely on analytical equations, we simulate real-world scenarios multiple times to estimate probabilities and distributions.

- **Random Walk**: 
  - A sequence of steps determined by random dice rolls.
  - Each roll updates the player's position, creating a "path" that evolves over time.
  - This concept is widely used in science, finance, and data modeling.
  - The random walk is dependent upon the previous steps to decide upon the current step. 

- **Monte Carlo Simulation**:
  - By simulating the game thousands of times, we can approximate the probability of reaching the target step.
  - The results form a **distribution** of final steps, which can be analyzed statistically.

- **Why Hacker Stats?**
  - Hacker stats allows us to bypass complex equations and directly simulate scenarios, making it a powerful tool for understanding random processes like this game.

---

## Features

- **Dynamic Random Walk Animation**:
  - Watch the player climb the steps dynamically in a smooth animated sequence.
  - The target step is highlighted to track progress visually.

- **Monte Carlo Simulation**:
  - Simulates thousands of random walks to estimate the probability of reaching the target step.
  - Results in a distribution of final steps, giving insights into the game's outcomes.

- **Interactive User Input**:
  - Specify the target step dynamically at runtime.

- **Statistical Analysis**:
  - Calculates and displays:
    - Probability of reaching the target step.
    - Mean, variance, and standard deviation of final steps.

- **Distribution Plot**:
  - A histogram visualizes the frequency of final steps across simulations.
  - Highlights the target step with a glittering gold dashed line.

---

## Setup

### Prerequisites

1. Python 3.7 or higher
2. Required libraries:
   ```bash
   pip install matplotlib numpy
   ```

### Installation

1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/HarshiniBorugadda/hacker-stats
   cd hacker-stats
   ```

---

## How to Run

1. Open the terminal and navigate to the project directory.
2. Create a notebook
3. Install the requirements
4. Enter the target step when prompted.

---

## Outputs

### 1. Dynamic Visualization

An animated sequence of a single random walk, showing:
- The player's movement dynamically over time.
- The target step highlighted in red.

**Example Output**:

<img src="https://github.com/user-attachments/assets/e206ce76-679c-4566-81f0-032dcf3a1fae" alt="Dynamic Visualization Example" width="600" height = "500">

---

### 2. Distribution Plot and Statistical Analysis

Histogram showing the distribution of final steps after all simulations:
- Target step highlighted with a **gold dashed line**.
- Frequency of final steps represented on the y-axis.
- **Probability** of reaching the target step.
- **Mean**, **variance**, and **standard deviation** of final steps.

**Example Output**:

<img src="https://github.com/user-attachments/assets/a1ccea64-c3f2-444c-96fb-9f09d5835005" alt="Statistical Analysis Output Example" width="800" height = "500">

---

## References

- [Monte Carlo Simulation](https://en.wikipedia.org/wiki/Monte_Carlo_method)
- [Random Walk](https://en.wikipedia.org/wiki/Random_walk)
- [Numpy for Statistical Calculations](https://numpy.org/doc/stable/reference/routines.statistics.html)
