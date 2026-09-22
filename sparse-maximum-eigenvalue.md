# Sparse maximum eigenvalue

↑ **Parent:** [Lasso](lasso.md)

For a [design matrix](design-matrix.md) $X$ with $p$ columns, define $\kappa_m^2=\max_{|M|=m}\lambda_{\max}(X_M^TX_M/n)$ for $1\le m\le p$. Equivalently this bounds $\|Xv\|_2^2/(n\|v\|_2^2)$ for [vectors](vector.md) supported on at most $m$ coordinates. These quantities are nondecreasing: extend the support of a maximizing [vector](vector.md) by zero coordinates and use the variational characterization of the largest [eigenvalue](eigenvalue.md). Values at $m>p$, including infinity, require a separate convention.

**Table of contents**

- [Lasso support bound from sparse eigenvalues](lasso-support-bound-from-sparse-eigenvalues.md)

## ↑ Ancestors (5)

1. [Lasso](lasso.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/2/solution.md)
