<h1 id="7g/solution">Solution</h1>

↑ **Parent:** [7G](../7g.md)

Orient the moving boundary $C(t)$ consistently with the normal on a spanning surface $S(t)$. The relevant [Maxwell equations](../../../../../maxwell-equations.md) are $\nabla\cdot\mathbf B=0$ and $\nabla\times\mathbf E=-\partial_t\mathbf B$.

First hold the magnetic field fixed at time $t$ and compare the fluxes through the old and new surfaces. The closed surface consists of the new surface, the reversed old surface, and the joining ribbon. A parametrization of the ribbon by boundary arclength and time gives its outward oriented area vector as $d\mathbf r\times\mathbf v\,\delta t$. Thus its flux is

$$
\int_{S'}\mathbf B\cdot d\mathbf S=-\delta t\oint_C\mathbf B\cdot(\mathbf v\times d\mathbf r).
$$

By the [divergence theorem](../../../../../divergence-theorem.md), the total flux through the closed surface is zero. Adding the field's explicit change in time consequently gives the moving-surface flux derivative

$$
\frac{d\Phi}{dt}=\int_{S(t)}\partial_t\mathbf B\cdot d\mathbf S+\oint_C\mathbf B\cdot(\mathbf v\times d\mathbf r).
$$

Now apply [Stokes theorem](../../../../../stokes-theorem.md) and $\mathbf B\cdot(\mathbf v\times d\mathbf r)=-(\mathbf v\times\mathbf B)\cdot d\mathbf r$:

$$
\frac{d\Phi}{dt}=-\oint_C\mathbf E\cdot d\mathbf r-\oint_C(\mathbf v\times\mathbf B)\cdot d\mathbf r.
$$

Consequently the [electromotive force](../../../../../electromotive-force.md), including the [motional electromotive force](../../../../../motional-electromotive-force.md), satisfies

$$
\boxed{\frac{d\Phi}{dt}=-\varepsilon.}
$$

This derives the moving-circuit form of [Faraday's law](../../../../../faraday-s-law-of-induction.md), including both changing fields and changing circuit geometry.

## ↑ Ancestors (10)

1. [7G](../7g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
