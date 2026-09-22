# Sparse dot product by merging indices

↑ **Parent:** [Dot product](dot-product.md)

For two [sparse vectors](sparse-vector.md) stored as increasing nonzero-coordinate streams, advance whichever current index is smaller; that coordinate has no possible partner in the other remaining stream. At equal indices, accumulate the product and advance both. The [loop invariant](loop-invariant.md) accounts for all matched coordinates already passed and excludes any future match for skipped smaller coordinates. Termination occurs when either stream ends. The method uses $O(k_1+k_2)$ time and constant [auxiliary space](auxiliary-space.md), with floating-point results subject to the chosen evaluation order.

## ↑ Ancestors (7)

1. [Dot product](dot-product.md)
2. [Inner product](inner-product-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/4/g/solution.md)
