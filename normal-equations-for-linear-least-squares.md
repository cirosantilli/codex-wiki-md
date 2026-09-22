# Normal equations for linear least squares

↑ **Parent:** [Linear regression](linear-regression-split.md)

Minimizing $\|y-X\theta\|^2$ gives the displayed equations by [differentiation](differentiation.md). Equivalently, the [regression residual](regression-residual.md) $r=y-X\widehat\theta$ satisfies $X^Tr=0$: it is [orthogonal](orthogonal-vectors.md) to every column of the [design matrix](design-matrix.md). If $X$ has [full column rank](full-column-rank.md), the minimizer is unique and the [fitted values](fitted-values.md) are the [orthogonal projection](orthogonal-projection.md) of $y$ onto its [column space](column-space.md). A rank-deficient [design matrix](design-matrix.md) can give multiple coefficient vectors, while the projected fitted vector is still unique.

For an [intercept](regression-intercept.md) and one predictor, put $S_{xx}=\sum_i(x_i-\bar x)^2$ and $S_{xy}=\sum_i(x_i-\bar x)(y_i-\bar y)$. The equations give $\widehat\beta=S_{xy}/S_{xx}$ and $\widehat\alpha=\bar y-\widehat\beta\bar x$, provided $S_{xx}>0$. In the five-point example in [linear regression](linear-regression-split.md), $\bar x=2$, $\bar y=2.8$, $S_{xx}=10$ and $S_{xy}=10$, giving $\widehat\beta=1$ and $\widehat\alpha=0.8$.

The [normal equations](normal-equation.md) describe the mathematical optimum, but explicitly forming and inverting $X^TX$ can amplify numerical problems. A [QR decomposition](qr-decomposition.md) computes the same [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) through orthogonal coordinates; a [singular value decomposition](singular-value-decomposition.md) also exposes nearly dependent columns. This connects statistical fitting to [numerical linear algebra](numerical-linear-algebra-split.md) and the choice of a stable algorithm. [MIT 18.06SC, Projections onto Subspaces and Least Squares](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/)

## ↑ Ancestors (8)

1. [Linear regression](linear-regression-split.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Linear least squares](linear-least-squares.md)
- [Log-linear exponential-decay fit](log-linear-exponential-decay-fit.md)
- [Orthogonal projection residual](orthogonal-projection-residual.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/18/b/ii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-c/c8/c/solution.md)
