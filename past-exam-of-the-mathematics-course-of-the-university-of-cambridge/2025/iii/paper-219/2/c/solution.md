<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take flat priors on $\alpha,\beta,\mu$ and scale priors $\pi(\sigma^2,\tau^2)\propto(\sigma^2\tau^2)^{-1}$ on the positive variances. The [posterior distribution](../../../../../../bayesian-posterior.md) is then

$$
\pi(\alpha,\beta,\sigma^2,\mu,\tau^2\mid\mathcal D)
\propto\frac{L(\alpha,\beta,\sigma^2,\mu,\tau^2)}{\sigma^2\tau^2}.
$$

A random-walk [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) can update $(\alpha,\beta,\mu,\log\sigma^2,\log\tau^2)$ with a symmetric proposal and accept a proposed state $z'$ from $z$ with probability $1\wedge\pi(z'\mid\mathcal D)/\pi(z\mid\mathcal D)$, including the Jacobian if the target is represented in transformed coordinates. Its transition kernel satisfies

$$
\pi(z)q(z,z')a(z,z')
=\min\{\pi(z)q(z,z'),\pi(z')q(z',z)\}
=\pi(z')q(z',z)a(z',z),
$$

which is [detailed balance](../../../../../../detailed-balance.md); hence the posterior is stationary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
