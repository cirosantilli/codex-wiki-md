# Recursive inverse of a lower triangular matrix

↑ **Parent:** [Lower triangular matrix](lower-triangular-matrix.md)

For an invertible [lower triangular matrix](lower-triangular-matrix.md), the scalar pivot $a$ and the remaining triangular block $C$ are both invertible. The displayed formula follows by [matrix multiplication](matrix-multiplication.md): the lower-left block in the product is $b/a-C(C^{-1}b/a)=0$, and the diagonal blocks are identities. Recursively invert $C$, compute $-C^{-1}b/a$, and assemble the [inverse matrix](matrix-inverse-split.md); the one-dimensional [base case](base-case.md) is $a^{-1}$. This [recursion](recursion-computer-science.md) reduces the size by one at each step.

## ↑ Ancestors (7)

1. [Lower triangular matrix](lower-triangular-matrix.md)
2. [Triangular matrix](triangular-matrix.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/3/b/solution.md)
