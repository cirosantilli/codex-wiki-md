# Condition-number bound for preconditioned steepest descent

↑ **Parent:** [Preconditioned steepest descent](preconditioned-steepest-descent.md)

Let $m=\lambda_{\min}(B)>0$, $L=\lambda_{\max}(B)$ and $\kappa=L/m=\kappa_2(B)$ for the transformed [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md). Then [preconditioned steepest descent](preconditioned-steepest-descent.md) satisfies

$$
E_{k+1}\le\left(\frac{\kappa-1}{\kappa+1}\right)^2E_k.
$$

This is a worst-case bound, not necessarily the actual rate. For our scaled example the bound is $(1/50)^2=0.0004$, slightly above its computed factor $q_M\approx0.000384321291$. If the initial transformed error is an [eigenvector](eigenvector.md), [exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md) removes it in one step, regardless of the full [condition number](condition-number.md).

A short proof compares [exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md) with the trial [step size](step-size.md) $\alpha=2/(m+L)$ in the transformed coordinates. In an [orthonormal eigenbasis](orthonormal-eigenbasis.md) of $B$, each error coefficient is multiplied by $1-\alpha\lambda_i$, whose [absolute value](absolute-value.md) is at most $(L-m)/(L+m)$. Summing $\lambda_i$ times the squared coefficients bounds the trial energy by the square of this factor. The exact minimizing [step size](step-size.md) does at least as well. This also explains the terminating case $m=L$: the trial step removes the entire error in one iteration.

## ↑ Ancestors (8)

1. [Preconditioned steepest descent](preconditioned-steepest-descent.md)
2. [Matrix preconditioning](matrix-preconditioning.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
