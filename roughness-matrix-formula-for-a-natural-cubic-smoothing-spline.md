# Roughness-matrix formula for a natural cubic smoothing spline

↑ **Parent:** [Cubic smoothing spline](cubic-smoothing-spline.md)

For distinct ordered observations $x_i$, let $s_u$ be their [natural cubic spline interpolant](natural-cubic-spline-interpolant.md) with values $u_i$. Its roughness is a [quadratic form](quadratic-form.md), $\int(s_u'')^2=u^TKu$, where $K$ is positive semidefinite and its nullspace consists of vectors sampled from affine functions. Minimizing [penalized least squares](penalized-least-squares.md) $\|y-u\|^2+\lambda u^TKu$ gives $\widehat u=(I+\lambda K)^{-1}y$. Thus the [smoothing matrix](smoothing-matrix.md) is $A_\lambda=(I+\lambda K)^{-1}$ and its [effective degrees of freedom](effective-degrees-of-freedom.md) are $\operatorname{tr}(A_\lambda)$. As $\lambda\downarrow0$ the fit approaches interpolation and the trace approaches $n$; as $\lambda\to\infty$ it approaches the least-squares affine line and the trace approaches $2$.

## ↑ Ancestors (9)

1. [Cubic smoothing spline](cubic-smoothing-spline.md)
2. [Smoothing spline](smoothing-spline.md)
3. [Nonparametric regression](nonparametric-regression.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43/5/c/solution.md)
