# Relative-entropy Lyapunov function for resource prices

↑ **Parent:** [Multiplicative resource-price dynamics](multiplicative-resource-price-dynamics.md)

For a complementary-slackness optimum $\mu^*$, define

$$
L(\mu)=\sum_j\kappa_j^{-1}[\mu_j-\mu_j^*-\mu_j^*\log(\mu_j/\mu_j^*)],
$$

interpreting a zero-reference summand as $\mu_j/\kappa_j$. This is a nonnegative generalized reverse-relative-entropy expression for positive resource prices. Along [multiplicative resource-price dynamics](multiplicative-resource-price-dynamics.md), with $p=A^T\mu$ and $g=Ax-C$,

$$
\dot L=-\sum_r\frac{w_r(p_r-p_r^*)^2}{p_rp_r^*}+\mu^Tg(\mu^*)\leq0.
$$

Its sublevel bounds keep all route prices away from zero and permit the [LaSalle invariance principle](lasalle-s-invariance-principle.md), including optima with some zero individual prices.

**Table of contents**

- [Full-row-rank convergence of multiplicative resource prices](full-row-rank-convergence-of-multiplicative-resource-prices.md)

## ↑ Ancestors (9)

1. [Multiplicative resource-price dynamics](multiplicative-resource-price-dynamics.md)
2. [Congestion control](congestion-control.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Full-row-rank convergence of multiplicative resource prices](full-row-rank-convergence-of-multiplicative-resource-prices.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39/4/solution.md)
