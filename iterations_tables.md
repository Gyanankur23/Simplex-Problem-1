# 🔁 Iteration Breakdown: Simplex Method

This file tracks the manual tableau transformations for **Simplex Problem 1**, including each pivot, basis update, and final optimal result.

---

## 🔢 Iteration 0: Initial Tableau

| C<sub>B</sub> | Basis | x₁ | x₂ | x₃ | s₁ | s₂ | s₃ | RHS |
|---------------|-------|----|----|----|----|----|----|-----|
| 0             | s₁    | 3  | 0  | 3  | 1  | 0  | 0  | 22  |
| 0             | s₂    | 1  | 2  | 3  | 0  | 1  | 0  | 14  |
| 0             | s₃    | 3  | 2  | 0  | 0  | 0  | 1  | 14  |

➡️ Entering Variable: **x₃** (Cj – Zj = 5)  
➡️ Leaving Variable: **s₂** (min ratio = 14 ÷ 3 = 4.67 approx)  
✅ Pivot Element = 3

---

## 🔢 Iteration 1: After Pivot on x₃ (s₂ leaves)

| C<sub>B</sub> | Basis | x₁   | x₂   | x₃ | s₁ | s₂     | s₃ | RHS    |
|---------------|-------|------|------|----|-----|--------|-----|--------|
| 0             | s₁    | 2    | -2   | 0  | 1   | -1     | 0   | 8      |
| 5             | x₃    | 1⁄3  | 2⁄3  | 1  | 0   | 1⁄3    | 0   | 14⁄3   |
| 0             | s₃    | 3    | 2    | 0  | 0   | 0      | 1   | 14     |

➡️ Entering Variable: **x₂**  
➡️ Leaving Variable: **x₃**  
✅ Pivot Element = 2⁄3

---

## 🔢 Iteration 2: After Pivot on x₂ (x₃ leaves)

| C<sub>B</sub> | Basis | x₁  | x₂ | x₃    | s₁ | s₂   | s₃ | RHS |
|---------------|-------|-----|----|--------|-----|-------|-----|-----|
| 0             | s₁    | 3   | 0  | 3      | 1   | 0     | 0   | 22  |
| 4             | x₂    | ½   | 1  | 3⁄2    | 0   | ½    | 0   | 7   |
| 0             | s₃    | 2   | 0  | -3     | 0   | -1    | 1   | 0   |

✅ All Cj – Zj ≤ 0 → Optimal solution reached  
📌 **Z = 28**

---

### 🧠 Pivot Summary

- Iteration 0 → Pivot on x₃ (s₂ leaves)  
- Iteration 1 → Pivot on x₂ (x₃ leaves)  
- Iteration 2 → Optimality confirmed, no further pivot

Every tableau marks a clear transformation using logic over code. These fractions aren’t just numbers—they’re strategy snapshots.
