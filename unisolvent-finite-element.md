# Unisolvent finite element

↑ **Parent:** [Finite element](finite-element.md)

A [finite element](finite-element.md) with local shape space $P$ and $n=\dim P$ [finite element degrees of freedom](finite-element-degree-of-freedom.md) $\ell_1,\ldots,\ell_n$ is unisolvent when each possible list of values determines exactly one member of $P$. By the [rank-nullity theorem](rank-nullity-theorem.md), it suffices to show that $\ell_i(p)=0$ for every $i$ implies $p=0$. Equivalently, one may construct a cardinal [basis](basis.md) $N_1,\ldots,N_n$ with $\ell_i(N_j)=\delta_{ij}$. Such a [basis](basis.md) is [linearly independent](linear-independence.md) by applying each $\ell_i$, and its size makes it span $P$; then $p=\sum_i\ell_i(p)N_i$.

## ↑ Ancestors (7)

1. [Finite element](finite-element.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite element degree of freedom](finite-element-degree-of-freedom.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/2/a/solution.md)
- [Quadratic Lagrange triangle](quadratic-lagrange-triangle.md)
