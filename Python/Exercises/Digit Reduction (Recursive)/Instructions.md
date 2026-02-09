# Digit Reduction (Recursive)

## Problem Description

Write a function that processes a list of **non‑negative integers** using recursive digit reduction.

---

## Requirements

### 1. Digit Reduction
For each integer in the list, replace it with the **sum of its digits**.

**Example:**
```

1234 → 1 + 2 + 3 + 4 = 10

```

---

### 2. Recursive Application
Repeat the digit‑sum process **recursively** on the entire list until **every element is a single digit (0–9)**.

---

### 3. Final Result
Once all elements are single digits, return the **maximum digit** in the list.

---

## Example

**Input**
`[1234, 567, 890]`

**Iteration 1**
`[10, 18, 17]`

**Iteration 2**
`[1, 9, 8]`

**Output**
`9`

---

## Notes

- Values that are already single digits should remain unchanged.
- Helper functions may be used, but the recursive logic must be part of the solution.
- Assume all input values are valid non‑negative integers.
