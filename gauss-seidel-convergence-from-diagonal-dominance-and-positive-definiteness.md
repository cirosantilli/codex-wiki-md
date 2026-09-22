# Gauss-Seidel convergence from diagonal dominance and positive definiteness

↑ **Parent:** [Gauss-Seidel method](gauss-seidel-method.md)

A [strictly diagonally dominant matrix](strictly-diagonally-dominant-matrix.md) or a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) guarantees convergence of the [Gauss-Seidel method](gauss-seidel-method.md) from every initial [vector](vector.md). These are sufficient conditions.[Math 221, Matrix Computations, Fall 2009; Theorem 1, strict row diagonal dominance, web lines 462–465; Theorem 3, positive-definite SOR and its ω = 1 specialization, web lines 490–493](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

For [strict diagonal dominance](strictly-diagonally-dominant-matrix.md), put

$$
q=\max_i\frac{\sum_{j\ne i}|a_{ij}|}{|a_{ii}|}<1,\qquad E=\|e^{(k)}\|_\infty.
$$

Induct through a sweep. Old coordinates have absolute error at most $E$; previously updated coordinates have absolute error at most $qE\leq E$. The component update and the [triangle inequality](triangle-inequality.md) therefore bound the new error by $qE$. This proves $\|e^{(k+1)}\|_\infty\leq q\|e^{(k)}\|_\infty$, a [maximum norm](supremum-norm.md) contraction.

For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), write $A=D+L+L^T$. The [Householder-John theorem](householder-john-theorem.md) applies to $M=D+L$ and $N=-L^T$, because $M^T+N=D$ is a [positive-definite matrix](positive-definite-matrix.md). Hence the [iteration matrix](iteration-matrix.md) has [spectral radius](spectral-radius.md) less than one, which gives the [convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md).

There is also a geometric reason fresh updates help: the [Gauss-Seidel method](gauss-seidel-method.md) is exact [coordinate descent](coordinate-descent.md) on the [convex quadratic function](convex-quadratic-function.md)

$$
F(z)=\frac12z^TAz-b^Tz,\qquad F(z)-F(x_*)=\frac12(z-x_*)^TA(z-x_*).
$$

Holding the other coordinates fixed, minimizing in coordinate $i$ gives the corresponding row update. A change $\delta_i$ lowers $F$ by exactly $a_{ii}\delta_i^2/2$. Each fresh coordinate is therefore the minimizer for the current [vector](vector.md), and a complete sweep lowers the [quadratic form](quadratic-form-split.md) error unless every coordinate already solves its row. This explains the method's beauty without implying monotone decrease in every [vector norm](norm.md).

**Table of contents**

- [Gauss-Seidel iteration can diverge for an invertible matrix](gauss-seidel-iteration-can-diverge-for-an-invertible-matrix.md)

## ↑ Ancestors (8)

1. [Gauss-Seidel method](gauss-seidel-method.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
