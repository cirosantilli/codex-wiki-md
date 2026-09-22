<h1 id="24h/solution">Solution</h1>

↑ **Parent:** [24H](../24h.md)

A covering map is locally a disjoint union of homeomorphisms onto the base. A space is simply connected when it is path-connected and every loop is null-homotopic. By the [uniformization theorem](../../../../../uniformization-theorem.md), the simply connected Riemann surfaces are

$$
\mathbb C_\infty,\qquad\mathbb C,\qquad\mathbb D
$$

up to analytic isomorphism.

A lattice is a discrete [subgroup](../../../../../subgroup.md)

$$
L=\mathbb Z\omega_1\oplus\mathbb Z\omega_2\subset\mathbb C
$$

with $\omega_1/\omega_2\notin\mathbb R$. The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md)

$$
\wp_L(z)=\frac1{z^2}+
\sum_{0\ne\omega\in L}
\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right)
$$

converges normally on compact subsets of $\mathbb C\setminus L$, defines a meromorphic map $\mathbb C\to\mathbb C_\infty$, and is nonconstant because it has a double pole at every lattice point. Reindexing the normally convergent [derivative](../../../../../derivative.md) [series](../../../../../series-mathematics.md) shows that $\wp_L'$ is $L$-periodic; evenness fixes the integration constants, so $\wp_L(z+\omega)=\wp_L(z)$.

The invariance makes

$$
\overline\wp([z])=\wp_L(z)
$$

well-defined and unique on $\mathbb C/L$. It is analytic because the quotient projection is locally biholomorphic.

Neither map is a covering. For any nonzero $\omega\in L$, periodicity and oddness of $\wp_L'$ give

$$
\wp_L'(\omega/2)=\wp_L'(-\omega/2)=-\wp_L'(\omega/2),
$$

so $\wp_L'(\omega/2)=0$. The map is not a local homeomorphism there; since the quotient projection is locally biholomorphic, the descended map fails for the same reason.

There is no covering $\mathbb C/L\to\mathbb C_\infty$. The torus is connected, while every connected covering of the simply connected sphere is a homeomorphism. A torus is not homeomorphic to a sphere, for example because their fundamental [groups](../../../../../group-split.md) are $\mathbb Z^2$ and $0$.

## ↑ Ancestors (10)

1. [24H](../24h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
