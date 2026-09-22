# Triangular solves for LU decomposition

↑ **Parent:** [LU decomposition](lu-decomposition.md)

Given [Pivoted LU decomposition](pivoted-lu-decomposition.md) $PA=LU$, the [linear system](system-of-linear-equations.md) $Ax=b$ is equivalent to $LUx=Pb$. Introduce the intermediate [vector](vector.md) $y=Ux$: first use [forward substitution](forward-substitution.md) to solve $Ly=Pb$, then [back substitution](back-substitution.md) to solve $Ux=y$. With unpivoted [LU decomposition](lu-decomposition.md), $P=I$ is the [identity matrix](identity-matrix.md), so the first right-hand side is simply $b$.[§2.4.4, equation (2.4.8) and Algorithm 2.4.2, and §2.6.3: two triangular solves and permutation of b](fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others.md)

For the factors in [Computed three-by-three LU decomposition](computed-three-by-three-lu-decomposition.md) and $b=(7,23,26)^T$, [forward substitution](forward-substitution.md) gives

$$
y_1=7,\qquad y_2=23-2(7)=9,\qquad y_3=26+7-3(9)=6.
$$

Then [back substitution](back-substitution.md) gives

$$
x_3=6/2=3,\qquad x_2=(9-3)/3=2,\qquad x_1=(7-2-3)/2=1.
$$

Direct [matrix multiplication](matrix-multiplication.md) verifies $A(1,2,3)^T=(7,23,26)^T$. More generally, the [back substitution](back-substitution.md) recurrence is

$$
x_i=\frac{y_i-\sum_{j=i+1}^{n}u_{ij}x_j}{u_{ii}},\qquad i=n,n-1,\ldots,1.
$$

The direction matters: the last row contains only $x_n$, whereas the first row generally involves every unknown. No dense [matrix inverse](matrix-inverse.md) is needed for either triangular solve.

**Table of contents**

- [Forward substitution](forward-substitution.md)

## ↑ Ancestors (7)

1. [LU decomposition](lu-decomposition.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
