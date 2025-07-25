# Subset Selection Problem 

This repository contains Python programs that solve the **Subset Sum Problem** under specific constraints using random sampling. The goal is to find all subsets from a given set of integers whose **sum is zero**.

---

## 🧩 Problem Statements

### 1. Fixed Subset Size = 5

- **Objective:** Find all unique subsets of size 5 whose elements sum to zero.
- **Set:**  {-12, -3, -6, 7, 2, -2, 6, 3, 9, -7, -5, -8, 1, 11, -9, -4}

- - **Method:** Randomly generate subsets and check if their sum is zero.
- **Output:** A set of tuples representing unique valid subsets.

### 2. Variable Subset Size (from 3 to 6)

- **Objective:** Find all unique subsets where the subset size ranges from 3 to 6 and the sum is zero.
- **Set:**  
{-12, -3, -6, 7, 2, -2, 6, 3, 9, -7, -5, -8, 1, 11, -9, -4}

- **Method:** Randomly select subset sizes and elements, check for zero-sum.
- **Output:** A set of tuples containing subsets of size 3–6 that sum to zero.

---

## 🚀 How It Works

- The algorithm uses `random.sample()` to generate subsets from the original set.
- It performs a specified number of iterations (e.g., 1000) to explore different combinations.
- Subsets that sum to zero are stored in a Python `set` to avoid duplicates.
- Subsets are sorted before being added to ensure uniqueness despite element order.

---

## 📁 Files

- `subset_fixed.py` – Program to find zero-sum subsets of size 5.
- `subset_variable.py` – Program to find zero-sum subsets of size 3 to 6.
- `README.md` – Project documentation.

---

## 🧪 Sample Output

### ✅ Fixed Subset Size (5)
```text
(-7, -4, 6, 3, 2)
(-5, 11, -8, 6, -4)
...
Total Sets: 16

(-5, 2, 3)
(-8, -4, 1, 11)
...
Total Sets: 14

