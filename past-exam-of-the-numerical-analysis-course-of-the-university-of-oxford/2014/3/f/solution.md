<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

[Strict diagonal dominance](../../../../strictly-diagonally-dominant-matrix.md) gives

$$
|b_{ii}|>\sum_{j\ne i}|b_{ij}|\geq0.
$$

Thus every $b_{ii}\ne0$, and the diagonal [matrix](../../../../matrix.md) $D$ has inverse $D^{-1}=\operatorname{diag}(1/b_{11},\ldots,1/b_{nn})$. The iteration [matrix](../../../../matrix.md) has entries

$$
t_{ii}=0,\qquad t_{ij}=\frac{b_{ij}}{b_{ii}}\quad(i\ne j).
$$

Each row [Gershgorin disc](../../../../gershgorin-disc.md) for $T$ is centred at zero and has radius

$$
\rho_i=\sum_{j\ne i}|t_{ij}|=\frac{\sum_{j\ne i}|b_{ij}|}{|b_{ii}|}<1.
$$

Therefore every [eigenvalue](../../../../eigenvalue.md) of $T$ satisfies

$$
\boxed{|\lambda|\leq\max_i\rho_i<1.}
$$

Equivalently, the induced [matrix norm](../../../../matrix-norm.md) satisfies $\|T\|_\infty<1$, bounding the [spectral radius](../../../../spectral-radius.md). This is the usual [Jacobi convergence from strict diagonal dominance](../../../../jacobi-convergence-from-strict-diagonal-dominance.md); the Jacobi error [matrix](../../../../matrix.md) is $-T$, with the same eigenvalue magnitudes.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
