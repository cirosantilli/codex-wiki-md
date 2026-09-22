<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A method-of-moments estimator uses

$$
\widehat r_1=\frac{\widehat\gamma(1)}{\widehat\gamma(0)}
\approx\frac{\theta}{1+\theta^2}.
$$

Under $|\theta|<1$, choose the invertible root

$$
\widehat\theta_{\mathrm{MM}}
=\frac{1-\sqrt{1-4\widehat r_1^2}}{2\widehat r_1},
$$

with the continuous value zero when $\widehat r_1=0$. Alternatively maximize the exact Gaussian likelihood using the positive-definite covariance matrix from part (i), producing $\widehat\theta_{\mathrm{ML}}$. Given either estimate,

$$
\widehat\sigma^2=\frac{\widehat\gamma(0)}{1+\widehat\theta^2}
$$

is the moment estimate; likelihood estimation may instead profile $\sigma^2$. Under a fixed interior parameter $|\theta|<1$ and standard stationary ergodic finite-moment regularity, both estimators are consistent and asymptotically normal, with Gaussian maximum likelihood asymptotically efficient.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
