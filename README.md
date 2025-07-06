# 🧮 Simplex Problem 1

Welcome to my first Linear Programming walkthrough using the Simplex Method. This manual approach breaks down optimization into digestible iterations, pivot decisions, and a clear narrative—no code, just clean math logic.

## 🧩 Problem Statement

**Objective Function:**  
Maximize: Z = x₁ + 4x₂ + 5x₃

**Subject to Constraints:**  
- x₁ − x₂ + x₃ ≤ 22  
- x₁ + 2x₂ + 3x₃ ≤ 14  
- 3x₁ + 2x₂ ≤ 14  
with x₁, x₂, x₃ ≥ 0

Converted to canonical form using slack variables:  
- x₁ − x₂ + x₃ + s₁ = 22  
- x₁ + 2x₂ + 3x₃ + s₂ = 14  
- 3x₁ + 2x₂ + 0x₃ + s₃ = 14

## 🔁 Methodology

✔ Manual Tableau Construction  
✔ Pivot Tracking by Cj – Zj values  
✔ Basis Updates per Iteration  
✔ Final Optimal Value Analysis

This project includes:
- Full tableau breakdown across 3 iterations  
- Slack interpretation  
- Z optimization logic  
- Visual insight into pivot movement

## 🎯 Final Solution

- x₂ = 7 (active variable)  
- Z = 28 (optimal value)  
- x₁, x₃, s₂ = 0 (non-basic)  
- s₁ = 22 and s₃ = 0 (slack interpretation)

## 📂 Files Included

- `iteration_tables.md` → All tableaux documented step-by-step  
- `simplex_notes.md` → Cheatsheet + interpretation notes  
- `diagrams/` → Visual assets (pivot flow, cheatsheet, banner)  
- `final_solution.txt` → Clean summary of variables and Z

## ✍️ Author

Crafted by **Gyanankur Baruah**  
Blending technical clarity with creative structure  
Linear Programming, decoded without code.
