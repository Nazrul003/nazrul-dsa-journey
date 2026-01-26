# LeetCode 73 – Set Matrix Zeroes (Row & Column Marker Intuition)

## Problem
If any cell in a matrix is `0`, set its **entire row and column** to `0`.
The update must be **in-place**.

---

## Core Idea (Intuition)

> One `0` affects many cells.  
> So first **remember where the zeros are**,  
> then **apply the effect everywhere**.

If we modify the matrix immediately, we lose original information.

---

## Approach (Two Pass Method)

### 1️⃣ First Pass – Mark (Do NOT modify matrix)
Create two marker arrays:
- `row[i]` → row `i` should become zero
- `col[j]` → column `j` should become zero

Initialize them with `1`.

While traversing the matrix:
```text
If matrix[i][j] == 0:
  row[i] = 0
  col[j] = 0
# LeetCode 73 – Set Matrix Zeroes (Row & Column Marker Intuition)

## Problem
If any cell in a matrix is `0`, set its **entire row and column** to `0`.
The update must be **in-place**.

---

## Core Idea (Intuition)

> One `0` affects many cells.  
> So first **remember where the zeros are**,  
> then **apply the effect everywhere**.

If we modify the matrix immediately, we lose original information.

---

## Approach (Two Pass Method)

### 1️⃣ First Pass – Mark (Do NOT modify matrix)
Create two marker arrays:
- `row[i]` → row `i` should become zero
- `col[j]` → column `j` should become zero

Initialize them with `1`.

While traversing the matrix:
```text
If matrix[i][j] == 0:
  row[i] = 0
  col[j] = 0
