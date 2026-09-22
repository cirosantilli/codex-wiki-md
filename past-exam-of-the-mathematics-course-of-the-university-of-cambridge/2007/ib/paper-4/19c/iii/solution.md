<h1 id="19c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $\mathbf e=\mathbf1/\sqrt n$ and $\mathbf f=\mathbf x/\sqrt{S_{xx}}$. These are orthonormal because $\sum_i x_i=0$. Complete them to an [orthonormal basis](../../../../../../orthonormal-basis.md) $\mathbf e,\mathbf f,\mathbf q_3,\ldots,\mathbf q_n$ of $\mathbb R^n$. An [orthogonal transformation](../../../../../../orthogonal-transformation.md) of the standard normal error vector $\boldsymbol\varepsilon/\sigma$ has independent [normal random variables](../../../../../../gaussian-random-variable.md) as coordinates $Z_1,\ldots,Z_n$: its [joint probability density](../../../../../../joint-probability-density.md) remains $(2\pi)^{-n/2}\exp(-\|z\|^2/2)$ because the transformation preserves squared length and has [Jacobian determinant](../../../../../../jacobian-determinant.md) of absolute value one.

Projection onto these [basis](../../../../../../basis.md) directions gives

$$
\widehat\alpha=\alpha+\frac\sigma{\sqrt n}Z_1,\qquad\widehat\beta=\beta+\frac\sigma{\sqrt{S_{xx}}}Z_2,\qquad\frac{\operatorname{RSS}}{\sigma^2}=\sum_{j=3}^nZ_j^2.
$$

Therefore the [joint distribution of least-squares and variance estimators](../../../../../../joint-distribution-of-least-squares-and-variance-estimators.md) is

$$
\boxed{\widehat\alpha\sim N(\alpha,\sigma^2/n),\quad\widehat\beta\sim N(\beta,\sigma^2/S_{xx}),\quad\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-2},\quad\text{all three independent}.}
$$

The last law is the [chi-squared distribution](../../../../../../chi-squared-distribution.md) of a sum of $n-2$ squared independent [normal random variables](../../../../../../gaussian-random-variable.md) with mean zero and variance one, and [independence](../../../../../../independent-random-variables.md) follows because the three statistics use disjoint independent coordinate sets. When all $x_i=0$, omit the slope direction: $\widehat\alpha$ and $n\widehat\sigma^2/\sigma^2\sim\chi^2_{n-1}$ are independent, and there is no identifiable slope estimator.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [19C](../../19c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
