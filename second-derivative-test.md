# Second-derivative test

↑ **Parent:** [Hessian matrix](hessian-matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second-derivative_test)

Let $f$ have continuous second [partial derivatives](partial-derivative.md) near an interior [critical point](critical-point.md) $x_*$ of an [open subset](open-set.md) of $\mathbb R^n$, with $\nabla f(x_*)=0$. The [Hessian matrix](hessian-matrix.md) gives the following sufficient conditions:
- All [eigenvalues](eigenvalue.md) positive: a strict [local minimum](local-minimum.md).
- All [eigenvalues](eigenvalue.md) negative: a strict [local maximum](local-maximum.md).
- Both positive and negative [eigenvalues](eigenvalue.md): a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md).

A [positive semidefinite](positive-semidefinite-matrix.md) or [negative semidefinite](negative-semidefinite-matrix.md) [Hessian matrix](hessian-matrix.md) with a zero [eigenvalue](eigenvalue.md) does not settle the classification. The [higher-order test for separated extrema](higher-order-test-for-separated-extrema.md) gives two quartic examples with exactly the same zero [Hessian](hessian-matrix.md). These conditions apply to an interior [critical point](critical-point.md); a boundary optimum or a [constrained optimization](constrained-optimization.md) problem requires attention to the allowed directions. [MIT 18.013A Calculus with Applications, §11.3: Hessian eigenvalues and the critical-point criterion](https://ocw.mit.edu/ans7870/18/18.013a/textbook/chapter11/section03.html)

The proof outline is the [Taylor expansion](taylor-expansion.md)

$$
f(x_*+h)-f(x_*)=\frac12h^TH_f(x_*)h+o(\|h\|^2).
$$

For a [positive-definite matrix](positive-definite-matrix.md), the smallest [eigenvalue](eigenvalue.md) supplies a positive bound proportional to $\|h\|^2$, which dominates the remainder for small enough $h$. Negate the [function](function-split.md) for the [local maximum](local-maximum.md) case. For opposite-sign [eigenvalues](eigenvalue.md), choose the two corresponding [eigenvectors](eigenvector.md): the leading terms have opposite signs along their lines.

There are also necessary conditions. At an interior [local minimum](local-minimum.md), the [Hessian matrix](hessian-matrix.md) is [positive semidefinite](positive-semidefinite-matrix.md); at an interior [local maximum](local-maximum.md), it is [negative semidefinite](negative-semidefinite-matrix.md). Restriction to each [straight line](straight-line.md) reduces this to the one-variable [second derivative](second-derivative.md) condition. Since the [Laplacian](laplacian.md) is the [trace](matrix-trace.md) of the [Hessian](hessian-matrix.md), it is nonnegative at such a [local minimum](local-minimum.md) and nonpositive at such a [local maximum](local-maximum.md). The sign of the [Laplacian](laplacian.md) alone is insufficient: $x^2-2y^2$ has negative [Laplacian](laplacian.md) but a [saddle point of a scalar function](saddle-point-of-a-scalar-function.md) at the origin.

**Table of contents**

- [Existence of second partial derivatives does not justify the Hessian test](existence-of-second-partial-derivatives-does-not-justify-the-hessian-test.md)
- [Critical points escaping to infinity in a Gaussian-weighted bilinear function](critical-points-escaping-to-infinity-in-a-gaussian-weighted-bilinear-function.md)

## ↑ Ancestors (8)

1. [Hessian matrix](hessian-matrix.md)
2. [Multivariable calculus](multivariable-calculus-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Existence of second partial derivatives does not justify the Hessian test](existence-of-second-partial-derivatives-does-not-justify-the-hessian-test.md)
- [Hessian matrix](hessian-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-313/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-2/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/16/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/16/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/12/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/14/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/12/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/12/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/12/e/solution.md)
- [Separable quartic landscape with nine stationary points](separable-quartic-landscape-with-nine-stationary-points.md)
