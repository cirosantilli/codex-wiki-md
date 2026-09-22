<h1 id="29j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gaussian likelihood](../../../../../../gaussian-likelihood.md) is proportional to

$$
\exp\!\left(-\frac{1}{2\sigma^2}\lVert Y-X\theta\rVert_2^2\right),
$$

so [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) is equivalent to [ordinary least squares](../../../../../../ordinary-least-squares.md). If $p\leq n$ and $X$ has [rank](../../../../../../rank-one-quadratic-form.md) $p$, then $X^TX$ is invertible and the [normal equations](../../../../../../normal-equation.md) give

$$
\boxed{\widehat\theta_{\rm MLE}=(X^TX)^{-1}X^TY.}
$$

If $p>n$, then $\operatorname{rank}X<p$ and $\ker X\ne\{0\}$. A least-squares minimizer always exists, but it is not unique: by [rank-deficient ordinary least squares](../../../../../../rank-deficient-ordinary-least-squares.md), the complete set is

$$
X^+Y+\ker X,
$$

an [affine subspace](../../../../../../affine-subspace.md) of dimension $p-\operatorname{rank}X>0$. Thus there are uncountably infinitely many likelihood maximizers. In the generic full-row-rank case their dimension is $p-n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
