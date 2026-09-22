<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply each time-sliced path weight by $\exp[-\sum_jV(x_j)\Delta t]$. A nonnegative finite $V$ is a local killing rate: the Feynman-Kac weight attenuates paths in proportion to the [time](../../../../../time-in-physics.md) spent in regions where $V>0$. Let that rate tend to infinity outside the allowed interval. Paths that exit are removed, leaving [Brownian motion](../../../../../brownian-motion-split.md) killed at its first boundary hit.

Consequently the required kernel is the Gaussian path measure restricted to surviving paths, equivalently

$$
\boxed{K_{|x|<L}
=\int_{x_i}^{x_f}\mathcal D x\,
e^{-\int[\dot x^2/(4D)+V(x)]dt},}
$$

with the infinite-barrier interpretation stated above. It solves $\partial_tK=D\partial_x^2K$ in the interior with absorbing [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) at $\pm L$. A [reflecting boundary condition for a diffusion](../../../../../reflecting-boundary-condition-for-a-diffusion.md) would describe a different process.

Strictly, this is a [transition probability](../../../../../transition-probability.md) density in the final [position](../../../../../position.md), jointly with survival; a [probability](../../../../../probability.md) for an interval of final [positions](../../../../../position.md) includes an integral over $x_f$. Its integral over the whole allowed interval is at most one. It is not the normalized endpoint density conditional on survival, which would require division by the [survival probability](../../../../../survival-probability.md). In these [diffusion](../../../../../diffusion.md) units $V$ and the [eigenvalues](../../../../../eigenvalue.md) of $H$ have units of inverse [time](../../../../../time-in-physics.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
