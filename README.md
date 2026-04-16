# AI61006 – Coding Assignment 1 (CasADi)

This repository contains the solution for **Coding Assignment 1** of the course  
**AI61006: Artificial Intelligence for Cyber Physical Systems**.

---

## 📌 Problem Description

The objective is to solve a constrained optimization problem using **CasADi** and the **IPOPT** solver.

### Optimization Problem

Minimize:
\[
f(x, y) = (y - 4x^2)^3
\]

Subject to:
\[
x^2 + 2y^2 = 4
\]
\[
x + y \leq 1
\]

---

## Methodology

- The objective function and constraints are defined using **CasADi symbolic expressions**
- The optimization problem is solved using the **IPOPT** solver
- A **contour plot** of the objective function is generated
- The **optimal solution** is marked on the contour plot
- The plot includes the **username and unique device ID**, as required

---

## Files

- `Assignment_1.ipynb` – Jupyter Notebook containing:
  - Problem formulation
  - Optimization using CasADi
  - Visualization and verification of optimal solution

---

## How to Run

1. Open `Assignment_1.ipynb`
2. Run all cells sequentially
3. Ensure the contour plot and optimal point are displayed

---

## Course Information

- **Course**: AI61006 – Artificial Intelligence for Cyber Physical Systems  
- **Assignment**: Coding Assignment 1  
- **Tool Used**: CasADi, IPOPT, Python

---

# SARSA Reinforcement Learning Assignment 2

---

## 📌 Assignment Overview
This assignment implements the **SARSA (State–Action–Reward–State–Action)** reinforcement learning algorithm using Gymnasium.  
The goal is to train an on-policy agent that learns an optimal policy through interaction with the environment using an epsilon-greedy strategy.

---

## Task Details

### Task 0 — Environment Setup
- Install required libraries (gymnasium, numpy, matplotlib, tqdm)
- Extract system information and generate a unique ID
- Embed ID and user name into plots for identification

---

### Task 1 — SARSA Implementation
- Implement epsilon-greedy policy for action selection
- Implement epsilon-greedy learning strategy
- Apply SARSA update rule to update Q-values
- Maintain Q-table for state-action learning

---

### Task 2 — Training the Agent
- Input student name for plot labeling
- Train the SARSA agent for multiple episodes
- Agent explores environment and updates policy
- Training performance plots are generated


---

### Task 3 — Testing / Evaluation
- Run the trained agent in inference mode
- Rendering enabled to visualize learned behaviour
- Used to verify effectiveness of learned policy


---

## How to Run
1. Open notebook in **Google Colab / Jupyter**
2. Run cells sequentially
3. First execute **training (Task 2)**
4. Then execute **testing (Task 3)**

---

## Algorithm Used

**SARSA Update Rule**

Where  
- `s` = current state  
- `a` = current action  
- `r` = reward  
- `s'` = next state  
- `a'` = next action  

---

# Newton-Based Reinforcement Learning

This project presents a **Newton-inspired modification of Q-learning**, where the traditional update rule is enhanced using a second-order approximation to achieve **faster and more stable convergence**.

---

## Overview

Reinforcement Learning (RL) algorithms like Q-learning typically rely on a **fixed learning rate**, which can lead to slow convergence or instability.

In this project, we introduce a **Newton-based update mechanism** that dynamically adapts the learning step using an approximation of the second-order derivative (Hessian).

---

## Key Idea

Instead of a constant learning rate, we scale updates using:

- Temporal Difference (TD) Error  
- Hessian approximation (second-order information)

This results in:

- Adaptive learning  
- Faster convergence  
- Improved stability  

---

## Algorithm

### 1. TD Error: δ = r + γ max Q(s', a') - Q(s, a)

### 2. Hessian Approximation: H ≈ |δ| + ε

### 3. Update Rule: Q(s, a) ← Q(s, a) + α * (δ / H)

---

---

## Implementation Details

- **Environment:** FrozenLake-v1 (Gymnasium)
- **Algorithm:** Newton-based Q-learning
- **Exploration:** Epsilon-greedy with decay
- **Episodes:** 10,000
- **Language:** Python

---

## Results

- **Success Rate:** 1.0  
- Rapid convergence after initial exploration  
- Stable performance across episodes  

The learning curve shows:
- Early exploration phase  
- Rapid improvement  
- Stable high reward region  

---

## 📁 Project Structure
Newton_RL/
│
├── newton_q_learning.ipynb
├── Newton_RL_Report.pdf
├── result.png In pdf
└── README.md

## Author
**Ravindra Mina**  
M.Tech Artificial Intelligence, IIT Kharagpur


