<h1 id="28l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A particle arriving at time $s\leq t$ survives until $t$ with probability $e^{-\mu(t-s)}$. Independently retaining each Poisson arrival with this time-dependent probability is [Poisson thinning](../../../../../../poisson-thinning.md). Hence the number alive at time $t$ is Poisson with mean

$$
\lambda\int_0^te^{-\mu(t-s)}ds
=\frac\lambda\mu(1-e^{-\mu t}).
$$

Thus

$$
\boxed{N_t^{\rm alive}\sim\operatorname{Poisson}\left(\frac\lambda\mu(1-e^{-\mu t})\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28L](../../28l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
