<h1 id="17h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the linear mean model as

$$
Y_i=\theta x_i+\varepsilon_i,
\qquad
\mathbb E\varepsilon_i=0,
\qquad
\operatorname{var}(\varepsilon_i)=\theta x_i.
$$

The errors are independent but [heteroscedastic](../../../../../../heteroscedastic.md). Minimizing the unweighted residual sum of squares

$$
Q(\theta)=\sum_{i=1}^n(Y_i-\theta x_i)^2
$$

gives the [normal equation](../../../../../../normal-equation.md)

$$
0=Q'(\theta)=-2\sum_i x_i(Y_i-\theta x_i).
$$

Thus, provided $\sum_i x_i^2>0$,

$$
\boxed{\widehat\theta_{LS}
=\frac{\sum_i x_iY_i}{\sum_i x_i^2}}.
$$

Since $\mathbb EY_i=\theta x_i$,

$$
\mathbb E\widehat\theta_{LS}
=\frac{\theta\sum_i x_i^2}{\sum_i x_i^2}=\theta.
$$

**Hence it is an [unbiased estimator](../../../../../../unbiased-estimator.md). This is the least-squares part of the [estimators for a Poisson exposure model](../../../../../../estimators-for-a-poisson-exposure-model.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17H](../../17h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
