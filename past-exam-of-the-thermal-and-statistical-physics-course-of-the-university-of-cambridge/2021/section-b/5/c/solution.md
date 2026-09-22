<h1 id="section-b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $M=\mathcal N=V/b$ for the number of cells; this is fixed even though the [particle](../../../../../particle-physics.md) number $N$ fluctuates. Approximate each position [integral](../../../../../integral-split.md) by the cell sum $\int d^3r_i\simeq b\sum_{\alpha_i=1}^M$, evaluating the slowly varying intercell [pair potential](../../../../../pair-potential.md) at cell centres. With the assumed single-occupancy restriction, the fixed-$N$ contribution becomes

$$
\frac1{N!}\left(\frac{e^{\beta\mu}b}{\lambda^3}\right)^N
\sum_{\alpha_1,\ldots,\alpha_N\ \mathrm{distinct}}
\exp\left[-\frac\beta2\sum_{i\ne j}\phi_{\alpha_i\alpha_j}\right].
$$

An occupation configuration $\{n_\alpha\}$ with $N=\sum_\alpha n_\alpha$ selects an unordered set of $N$ occupied cells. There are exactly $N!$ ways to assign the temporary [particle](../../../../../particle-physics.md) labels to that set. They all have the same interaction [energy](../../../../../energy-split.md), cancelling the prefactor $1/N!$.

Summing over all [particle](../../../../../particle-physics.md) numbers is therefore equivalent to summing each cell occupation independently over $0,1$:

$$
\boxed{\Xi\simeq\sum_{n_1=0}^1\cdots\sum_{n_M=0}^1
\left(\frac{e^{\beta\mu}b}{\lambda^3}\right)^{\sum_\alpha n_\alpha}
\exp\left[-\frac\beta2\sum_{\alpha\ne\alpha'}n_\alpha n_{\alpha'}\phi_{\alpha\alpha'}\right].}
$$

The activity per cell, $e^{\beta\mu}b/\lambda^3$, is dimensionless. This is a [lattice gas](../../../../../lattice-gas.md), with each cell either empty or occupied.

The exclusion of multiple occupation is an additional physical modeling assumption, explicitly imposed by the question. Making a cell small does not by itself forbid two point [particles](../../../../../particle-physics.md) from entering it; a repulsive core or a dilute-occupancy approximation would be needed to justify that restriction starting from a general continuum [pair potential](../../../../../pair-potential.md). In the remaining parts it is part of the defined cell model.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
