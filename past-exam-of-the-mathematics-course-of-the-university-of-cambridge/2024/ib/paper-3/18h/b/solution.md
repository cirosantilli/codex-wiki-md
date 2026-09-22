<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditionally on $\mu$,

$$
\overline X\mid\mu\sim N\left(\mu,\frac1n\right),
$$

so

$$
\boxed{
f(\overline x\mid\mu)
=\sqrt{\frac n{2\pi}}
\exp\left[-\frac n2(\overline x-\mu)^2\right]}.
$$

Under the continuous half of the prior, write $\overline X=\mu+Z$ with independent

$$
\mu\sim N(0,\tau^2),
\qquad
Z\sim N(0,1/n).
$$

Thus $\overline X\sim N(0,\tau^2+1/n)$ there. Mixing this density with the point-null density gives the [marginal likelihood for a Gaussian point-null mixture](../../../../../../marginal-likelihood-for-a-gaussian-point-null-mixture.md)

$$
\boxed{
\begin{aligned}
m(\overline x)={}&\frac12\sqrt{\frac n{2\pi}}
 e^{-n\overline x^2/2}\\
&+\frac1{2\sqrt{2\pi(\tau^2+1/n)}}
 \exp\left[-\frac{\overline x^2}{2(\tau^2+1/n)}\right].
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
