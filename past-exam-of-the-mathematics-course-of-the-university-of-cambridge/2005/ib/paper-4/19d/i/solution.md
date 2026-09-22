<h1 id="19d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $S_{xx}=\sum_i x_i^2>0$, which is necessary to identify the slope in [linear regression through the origin](../../../../../../linear-regression-through-the-origin.md). The joint normal likelihood has logarithm, apart from a constant,

$$
\ell(\beta,\sigma^2)=-\frac n2\log\sigma^2-\frac1{2\sigma^2}\sum_i(Y_i-\beta x_i)^2.
$$

Complete the square in $\beta$. With $\widehat\beta=\sum_i x_iY_i/S_{xx}$ and $\mathrm{RSS}=\sum_i(Y_i-\widehat\beta x_i)^2$,

$$
\sum_i(Y_i-\beta x_i)^2=\mathrm{RSS}+S_{xx}(\beta-\widehat\beta)^2.
$$

The [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) therefore first minimizes at $\widehat\beta$; differentiating in $\sigma^2$ then maximizes at

$$
\boxed{\widehat\beta=\frac{\sum_i x_iY_i}{S_{xx}},\qquad \widehat\sigma^2=\frac{\mathrm{RSS}}n.}
$$

This is a genuine finite maximum when $\mathrm{RSS}>0$. If all $x_i=0$, the slope is unidentifiable. If $\mathrm{RSS}=0$, the likelihood is unbounded as $\sigma^2\downarrow0$, so no positive-variance maximum exists. For nonzero design and $n\geq2$, zero residual has probability zero under the stated positive-variance model.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19D](../../19d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
