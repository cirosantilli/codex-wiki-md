# Discrete orthogonality of Gaussian quadrature

↑ **Parent:** [Gaussian quadrature](gaussian-quadrature.md)

Let $\phi_0,\ldots,\phi_n$ be [orthonormal](orthonormal-set.md) [polynomials](polynomial-split.md) for a positive weight, and let $x_i,w_i$ define its $(n+1)$-point [Gaussian quadrature](gaussian-quadrature.md). Put $A_{ij}=\phi_{j-1}(x_{i-1})$ and $W=\operatorname{diag}(w_0,\ldots,w_n)$. Exactness through [polynomial degree](degree-of-a-polynomial.md) $2n+1$ gives $A^TWA=I$. Positivity of the [quadrature weights](quadrature-weight.md) makes $W^{1/2}A$ a square [orthogonal matrix](orthogonal-matrix.md), so $AA^T=W^{-1}$ also. Thus the unweighted row [inner products](inner-product-split.md) of the evaluation [matrix](matrix.md) are $\delta_{ij}/w_{i-1}$.

## ↑ Ancestors (6)

1. [Gaussian quadrature](gaussian-quadrature.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2021/1/c/iii/solution.md)
