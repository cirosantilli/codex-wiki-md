# Exponential-linear separable potential

↑ **Parent:** [Critical point](critical-point.md)

Let $a_i,c_i$ be nonzero real constants with $a_ic_i>0$. The real [function](function-split.md) $H:\mathbb R^n\to\mathbb R$ displayed in the title has exactly one [stationary point](stationary-point.md):

$$
x_i^*=\log(c_i/a_i),\qquad
H(x^*)=\sum_i\bigl[c_i-c_i\log(c_i/a_i)\bigr].
$$

Indeed the [partial derivatives](partial-derivative.md) are $a_i e^{x_i}-c_i$, each of which has precisely one zero. The [Hessian matrix](hessian-matrix.md) at that point is $\operatorname{diag}(c_1,\ldots,c_n)$.

If every $c_i>0$, each summand is a [strictly convex function](strictly-convex-function.md) tending to $+\infty$ as its argument tends to either infinity. Consequently $H$ has a unique [global minimum](global-minimum.md). If every $c_i<0$, negating $H$ gives the preceding case, proving a unique [global maximum](global-maximum.md). If both signs occur, restricting to two coordinate directions of opposite signs gives a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md). No degenerate [Hessian matrix](hessian-matrix.md) is possible under the nonzero assumptions.

## ↑ Ancestors (5)

1. [Critical point](critical-point.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
