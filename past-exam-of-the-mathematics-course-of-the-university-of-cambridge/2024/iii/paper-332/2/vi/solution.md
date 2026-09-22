<h1 id="2/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The approximation in part v requires the dimensionless stagnant depth

$$
\eta=
\frac{1-3\theta/5}
{\mathcal F\theta^{5/3}}
$$

to remain small. Since $0<\theta\leq1$ makes the numerator order one, this condition is

$$
\boxed{\theta\gg\mathcal F^{-3/5}}.
$$

Using the solution from part v, the equivalent time range is

$$
1+\frac23\mathcal F\tau
\ll\mathcal F^{2/5},
$$

or, at the level of [asymptotic equivalence](../../../../../../asymptotic-equivalence.md),

$$
\boxed{0\leq\tau\ll\mathcal F^{-3/5}}.
$$

The cooling becomes appreciable on the shorter scale $\tau=O(\mathcal F^{-1})$, so these ranges overlap widely when $\mathcal F\gg1$.

The [Rayleigh number](../../../../../../rayleigh-number.md) based on the convecting depth is

$$
\operatorname{Ra}
=\frac{g\alpha(T_w-T_m)^2(H-h)^3}{\nu\kappa}.
$$

The definition of $\mathcal F$ implicit in part iii gives

$$
\mathcal F
=C_0H
\left(\frac{g\alpha\Delta T^2}
{\operatorname{Ra}_c\nu\kappa}\right)^{1/3}.
$$

It follows that

$$
\boxed{
\operatorname{Ra}
=\operatorname{Ra}_c
\left(\frac{\mathcal F}{C_0}\right)^3
\theta^2(1-\eta)^3}.
$$

If $1-\eta=O(1)$ and $\theta\gg\mathcal F^{-3/5}$, then $\operatorname{Ra}\gg O(\mathcal F^{9/5})$. The [thermal convection](../../../../../../thermal-convection.md) therefore remains strongly supercritical throughout the range in which the thin stagnant-layer approximation is valid.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
