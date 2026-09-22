<h1 id="5l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditionally on $x_i$,

$$
\mathbb P(Z_i=1\mid x_i)
=\Phi\left(\frac{\mu+x_i^T\beta-\tau}{\sigma}\right).
$$

Thus this is a probit regression with linear predictor

$$
\eta_i=\alpha+x_i^T\gamma,
\qquad \alpha=\frac{\mu-\tau}{\sigma},
\qquad \gamma=\frac\beta\sigma.
$$

Fit $(\alpha,\gamma)$ by maximum likelihood for Bernoulli observations, then recover

$$
\widehat\mu=\tau+\sigma\widehat\alpha,
\qquad \widehat\beta=\sigma\widehat\gamma.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5L](../../5l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
