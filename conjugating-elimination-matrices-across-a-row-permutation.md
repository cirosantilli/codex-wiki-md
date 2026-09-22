# Conjugating elimination matrices across a row permutation

↑ **Parent:** [Pivoted LU decomposition](pivoted-lu-decomposition.md)

For a [permutation matrix](permutation-matrix.md) $P$ and elimination [matrices](matrix.md) $E_i$, put $F_i=PE_iP^{-1}$. Cancellation of adjacent $P^{-1}P$ gives $PE_k\cdots E_1M=F_k\cdots F_1(PM)$. If the $F_i$ and their inverses are lower triangular, then $PM=LU$ with $U=PE_k\cdots E_1M$ and $L=F_1^{-1}\cdots F_k^{-1}$. Lower triangularity needs checking: an arbitrary permutation does not preserve it.

## ↑ Ancestors (8)

1. [Pivoted LU decomposition](pivoted-lu-decomposition.md)
2. [LU decomposition](lu-decomposition.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/digital-systems-linear-algebra-introduction-to-formal-proof/5/c/solution.md)
