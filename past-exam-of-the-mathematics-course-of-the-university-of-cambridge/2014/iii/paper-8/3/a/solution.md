<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [transport cost](../../../../../../transport-cost-function.md) separates into a [function](../../../../../../function-split.md) of $y$ and a [function](../../../../../../function-split.md) of $x$, so for every [transport plan](../../../../../../transport-plan.md)

$$
\int(y-x)\,d\pi=\int_1^2 y\,d\nu(y)-\int_0^1 x\,d\mu(x).
$$

The value is fixed by the marginals. Hence **every [transport map](../../../../../../transport-map.md) from $\mu$ to $\nu$ is optimal**, and indeed every coupling is optimal.

For an explicit description of the complete set, let $F(x)=\int_0^x f(s)\,ds$ and $G(y)=\int_1^y g(s)\,ds$. Their strictly positive continuous densities make $F:[0,1]\to[0,1]$ and $G:[1,2]\to[0,1]$ increasing homeomorphisms. The full family of deterministic plans is

$$
\boxed{\pi_T=(\operatorname{Id},T)_*\mu,\qquad
T=G^{-1}\circ S\circ F\quad\mu\text{-almost everywhere},}
$$

where $S:[0,1]\to[0,1]$ is any measurable [Lebesgue-measure-preserving map](../../../../../../lebesgue-measure-preserving-map.md). Indeed $F_*\mu$ is uniform [measure](../../../../../../measure.md) and $G_*\nu$ is uniform [measure](../../../../../../measure.md), so any such $S$ produces the required pushforward. Conversely, for any [transport map](../../../../../../transport-map.md) $T$, the map $S=G\circ T\circ F^{-1}$ preserves uniform [measure](../../../../../../measure.md). This is the [measure-preserving parametrization of one-dimensional transport maps](../../../../../../measure-preserving-parametrization-of-one-dimensional-transport-maps.md); no monotonicity is required for the linear cost.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
