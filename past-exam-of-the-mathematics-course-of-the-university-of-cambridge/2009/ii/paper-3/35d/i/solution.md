<h1 id="35d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Measure energy from the single-particle ground state and write $z=e^{\mu/(k_BT)}\le1$. The [Bose-Einstein distribution](../../../../../../bose-einstein-distribution.md) gives the number in excited levels as

$$
N_{\mathrm{ex}}=B\int_0^\infty\frac{\epsilon^{7/2}}{z^{-1}e^{\epsilon/(k_BT)}-1}d\epsilon
=B\Gamma(\tfrac92)(k_BT)^{9/2}\operatorname{Li}_{9/2}(z).
$$

Here $\operatorname{Li}_s(z)=\sum_{j\ge1}z^j/j^s$, obtained directly from the supplied integral identity. At the [Bose-Einstein condensation](../../../../../../bose-einstein-condensation.md) threshold, $z\uparrow1$ and the excited states are just able to hold all $N$ particles. Thus

$$
\boxed{T_c=\frac1{k_B}\left[\frac{N}{B\Gamma(9/2)\zeta(9/2)}\right]^{2/9}.}
$$

The ground-state population is treated separately from the continuum [density of states](../../../../../../density-of-states.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [35D](../../35d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
