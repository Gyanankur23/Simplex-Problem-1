# 🧠 Simplex Method Notes & Reflections

This markdown captures lessons, strategic shortcuts, and intuitive thinking behind the manual walkthrough of **Simplex Problem 1**. It’s not just about solving—it’s about understanding.

---

## 🧩 Core Concepts (Mini Cheatsheet)

- **Objective Function:** Maximize Z with decision variables (x₁, x₂, x₃)
- **Constraints → Equations:** Add slack variables to convert "≤" into equations
- **Basic & Non-Basic Variables:** Track which variables are in the basis at every stage
- **Pivot Logic:**  
  - Entering Variable → Column with highest Cj – Zj  
  - Leaving Variable → Row with minimum RHS ÷ Pivot Column Entry
- **Optimality Check:** All Cj – Zj ≤ 0 → You’ve reached max Z

---

## 🔄 Iteration Reflections

### Iteration 0  
- Tableau initialized with slack variables s₁, s₂, s₃  
- Highest gain from x₃ → selected to enter  
- s₂ leaves basis → it contributes least per unit of x₃

### Iteration 1  
- x₃ enters → new row formed  
- Cj – Zj check highlights x₂ as next candidate  
- s₁, s₃ stay unchanged but RHS shifts

### Iteration 2  
- x₂ enters, x₃ leaves  
- x₂ becomes basic and unlocks Z = 28  
- No further positive Cj – Zj → Optimal solution confirmed

---

## 🧮 Slack Variable Insights

- s₁ = 22 → First constraint still has leftover capacity  
- s₂ = 0 → Fully utilized when it left the basis  
- s₃ = 0 → Third constraint tightly bounds solution

Slack variables reveal how far each constraint is from being “tight.” Zero slack means the constraint directly shapes the solution boundary.

---

## 📘 Learnings for Future LP Problems

- Always convert constraints cleanly—bad canonical form creates confusion  
- Pivot calculations are easier with fractions than decimals (don’t rush to convert)  
- Tableau snapshots clarify logic more than formulas  
- Manual walkthrough builds intuition better than automated output  
- Final interpretation matters—don’t just find Z, explain it

---
