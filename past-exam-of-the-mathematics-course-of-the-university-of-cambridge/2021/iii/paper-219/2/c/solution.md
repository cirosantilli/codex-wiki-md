<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The posterior is

$$
p(\mu,\theta\mid y,t)\propto
p(y\mid t;\mu,\theta)p(\mu,\theta).
$$

A random-walk [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) proposes $\vartheta'$ from a symmetric density about the current $\vartheta=(\mu,\theta)$ and accepts with probability

$$
a(\vartheta,\vartheta')
=\min\left\{1,\frac{p(\vartheta'\mid y,t)}{p(\vartheta\mid y,t)}\right\}.
$$

For distinct states, multiplying the transition density by the target density gives

$$
p(\vartheta\mid y,t)q(\vartheta'\mid\vartheta)a(\vartheta,\vartheta')
=\min\{p(\vartheta\mid y,t)q,\ p(\vartheta'\mid y,t)q\},
$$

which is symmetric and proves [detailed balance](../../../../../../detailed-balance.md). Run multiple dispersed chains, tune proposals during warm-up, inspect traces, effective sample sizes and convergence diagnostics, then estimate the period mean by averaging $2\pi/\omega_m$ over retained draws.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
