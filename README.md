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

## 🛠️ Methodology

- The objective function and constraints are defined using **CasADi symbolic expressions**
- The optimization problem is solved using the **IPOPT** solver
- A **contour plot** of the objective function is generated
- The **optimal solution** is marked on the contour plot
- The plot includes the **username and unique device ID**, as required

---

## 📁 Files

- `Assignment_1.ipynb` – Jupyter Notebook containing:
  - Problem formulation
  - Optimization using CasADi
  - Visualization and verification of optimal solution

---

## ▶️ How to Run

1. Open `Assignment_1.ipynb`
2. Run all cells sequentially
3. Ensure the contour plot and optimal point are displayed

---

## 🧑‍🎓 Course Information

- **Course**: AI61006 – Artificial Intelligence for Cyber Physical Systems  
- **Assignment**: Coding Assignment 1  
- **Tool Used**: CasADi, IPOPT, Python

---

