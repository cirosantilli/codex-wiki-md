<h1 id="28l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
\bar z=\frac1n\sum_{i=1}^nz_i,
\qquad
S(\mu)=\sum_{i=1}^n(z_i-\mu)^2.
$$

Multiplying the likelihood by the [improper prior](../../../../../../improper-prior.md) gives the [Bayesian posterior](../../../../../../bayesian-posterior.md) kernel

$$
\pi(\mu,\omega\mid z)
\propto
\omega^{n/2}
\exp\left\{-\omega\left(\lambda+\frac12S(\mu)\right)\right\},
\qquad \omega>0.
$$

Since

$$
S(\mu)=\sum_{i=1}^n(z_i-\bar z)^2+n(\mu-\bar z)^2,
$$

the first full conditional is

$$
\boxed{\mu\mid\omega,z\sim
N\left(\bar z,\frac1{n\omega}\right)}.
$$

Holding $\mu$ fixed and comparing powers and exponential rates gives

$$
\boxed{\omega\mid\mu,z\sim
\operatorname{Gamma}\left(
m,\lambda+\frac12S(\mu)\right)},
\qquad
m=\frac n2+1.
$$

The assumed parity of $n$ makes $m$ a positive integer.

Initialize $\mu_0$ arbitrarily. At iteration $j$, put

$$
r_j=\lambda+\frac12S(\mu_{j-1}).
$$

Draw $m$ independent uniform variables $U_{j1},\ldots,U_{jm}$ and set

$$
\omega_j=-\frac1{r_j}\sum_{\ell=1}^m\log U_{j\ell}.
$$

By [sampling an integer-shape gamma distribution](../../../../../../sampling-an-integer-shape-gamma-distribution.md), this has the required $\operatorname{Gamma}(m,r_j)$ law. Next draw $G_j\sim N(0,1)$ independently and set

$$
\mu_j=\bar z+\frac{G_j}{\sqrt{n\omega_j}}.
$$

These are exactly the two full-conditional updates of the [normal mean-precision Gibbs sampler](../../../../../../normal-mean-precision-gibbs-sampler.md). After discarding burn-in, the pairs $(\mu_j,\omega_j)$ are approximate samples from the posterior by [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28L](../../28l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
