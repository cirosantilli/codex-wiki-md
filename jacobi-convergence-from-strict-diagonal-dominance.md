# Jacobi convergence from strict diagonal dominance

↑ **Parent:** [Jacobi method](jacobi-method.md)

A [strictly diagonally dominant matrix](strictly-diagonally-dominant-matrix.md) guarantees convergence of the [Jacobi method](jacobi-method.md) for every initial [vector](vector.md).[Math 221, Matrix Computations, Fall 2009; Theorem 1 on strict row diagonal dominance and its proof beginning “Split A = D − (D − A)”](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

Indeed, using the [maximum norm](supremum-norm.md) $\|v\|_\infty=\max_i|v_i|$, the induced [operator norm](operator-norm.md) is the largest absolute row sum. The [Jacobi method](jacobi-method.md) has $b_{ii}=0$ and $b_{ij}=-a_{ij}/a_{ii}$ for $j\ne i$, so

$$
\rho(B)\leq\|B\|_\infty=\max_i\frac{\sum_{j\ne i}|a_{ij}|}{|a_{ii}|}<1,\qquad \|e^{(k)}\|_\infty\leq\|B\|_\infty^k\|e^{(0)}\|_\infty.
$$

This gives a cheap sufficient check without computing any [eigenvalues](eigenvalue.md). For the [Jacobi iteration for a three-variable tridiagonal system](jacobi-iteration-for-a-three-variable-tridiagonal-system.md), the absolute row sums of $B$ are $1/4,1/2,1/4$, giving $\|B\|_\infty=1/2$. The true [spectral radius](spectral-radius.md) $\sqrt2/4$ gives a sharper eventual rate.

Strict [diagonal dominance](diagonal-dominance.md) is sufficient, not necessary: $A=\begin{pmatrix}1&2\\1/10&1\end{pmatrix}$ violates it in the first row, but its [Jacobi method](jacobi-method.md) has [eigenvalues](eigenvalue.md) $\pm1/\sqrt5$ and converges. Conversely, being a [positive-definite matrix](positive-definite-matrix.md) alone is insufficient: the [Jacobi convergence for a three-by-three equicorrelation matrix](jacobi-convergence-for-a-three-by-three-equicorrelation-matrix.md) with $\alpha=3/4$ has positive [eigenvalues](eigenvalue.md) $5/2,1/4,1/4$ for $A$, but [spectral radius](spectral-radius.md) $3/2$ for its [iteration matrix](iteration-matrix.md). The extra [tridiagonal matrix](tridiagonal-matrix.md) structure in [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix.md) is therefore substantive.

## ↑ Ancestors (8)

1. [Jacobi method](jacobi-method.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
