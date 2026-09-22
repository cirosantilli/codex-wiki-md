<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [invariance property of maximum likelihood estimation](../../../../../../invariance-property-of-maximum-likelihood-estimation.md) gives

$$
\widehat h=10^{\widehat\theta/5}
=\exp(\widehat\theta/\alpha).
$$

Since $\widehat\theta-\theta\sim N(0,\sigma_\theta^2)$, the ratio $\widehat h/h$ has a [log-normal distribution](../../../../../../log-normal-distribution.md). Its exact variance is

$$
\operatorname{Var}\!\left(\frac{\widehat h}{h}\right)
=e^{\sigma_\theta^2/\alpha^2}
\left(e^{\sigma_\theta^2/\alpha^2}-1\right),
$$

and the lowest-order [delta method](../../../../../../delta-method.md) approximation is

$$
\operatorname{Var}\!\left(\frac{\widehat h}{h}\right)
=\frac{\sigma_\theta^2}{\alpha^2}+O(\sigma_\theta^4).
$$

For fixed $\sigma_{\rm tot}$, case (i) has $A=\sigma_\mu^2+\sigma_{\rm tot}^2$, whereas case (ii) has $A=\sigma_\mu^2+\sigma_{\rm tot}^2/K$. Because $K\geq2$ and $B$ is the same in both cases, independent supernova-level variation in case (ii) gives the smaller fractional variance: averaging reduces it, while a shared galaxy fluctuation does not average away.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
