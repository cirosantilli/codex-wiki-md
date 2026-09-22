<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

For $Y_\mu\sim\operatorname{Poisson}(\mu)$, the [delta method](../../../../../delta-method.md) with $g(y)=2\sqrt y$ gives

$$
\operatorname{Var}(g(Y_\mu))
\approx g'(\mu)^2\operatorname{Var}(Y_\mu)
=\frac1\mu\mu=1.
$$

Thus the transformation stabilizes variance at large $\mu$.

A Gaussian linear model for $\sqrt Y$ treats the transformed observations as having additive constant-variance errors and models $\mathbb E(\sqrt Y\mid X)$ as linear. A [Poisson regression](../../../../../poisson-regression.md) with square-root link retains the Poisson likelihood and models

$$
\sqrt{\mathbb E(Y\mid X)}=X\beta.
$$

The two procedures therefore have different likelihoods, fitted means, and constraints; transforming the response is not the same as transforming its conditional mean.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
