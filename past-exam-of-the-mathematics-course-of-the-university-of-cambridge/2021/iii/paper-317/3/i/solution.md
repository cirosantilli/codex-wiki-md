<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the mean interior density as

$$
\bar\rho(r)=\frac{3m_r}{4\pi r^3}.
$$

Since

$$
\frac{d\bar\rho}{dr}=\frac3r(\rho-\bar\rho),
$$

the assumed outward decrease of $\bar\rho$ implies $\rho\leq\bar\rho$. In mass coordinates, [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) is

$$
\frac{dP}{dm_r}=-\frac{Gm_r}{4\pi r^4}
=-\frac G3\left(\frac{4\pi}{3}\right)^{1/3}
\bar\rho^{4/3}m_r^{-1/3}.
$$

For every interior mass $m\leq m_r$, monotonicity gives

$$
\bar\rho(r)\leq\bar\rho(m)\leq\rho_c.
$$

Integrating from the centre and using $\int_0^{m_r}m^{-1/3}dm=3m_r^{2/3}/2$ proves

$$
\boxed{\frac G2\left(\frac{4\pi}{3}\right)^{1/3}
\bar\rho^{4/3}m_r^{2/3}
\leq P_c-P(r)\leq
\frac G2\left(\frac{4\pi}{3}\right)^{1/3}
\rho_c^{4/3}m_r^{2/3}}.
$$

Let $\mathcal R$ be the gas constant per mole. At the centre,

$$
\beta_cP_c=\frac{\mathcal R}{\mu}\rho_cT_c,
\qquad
(1-\beta_c)P_c=\frac{aT_c^4}{3}.
$$

Eliminating $T_c$ gives the [Eddington quartic relation](../../../../../../eddington-quartic-relation.md) in its central form,

$$
\boxed{\frac{1-\beta_c}{\beta_c^4}
=\frac a3\left(\frac{\mu}{\mathcal R}\right)^4
\frac{P_c^3}{\rho_c^4}}.
$$

At the surface, set $P=0$ and $m_r=M$ in the upper pressure bound. Cubing it gives

$$
\frac{P_c^3}{\rho_c^4}\leq\frac{\pi}{6}G^3M^2.
$$

The function $(1-\beta)/\beta^4$ decreases strictly as $\beta$ increases on $0<\beta<1$. Define $\beta^*$ by equality in the resulting bound:

$$
\frac{1-\beta^*}{\beta^{*4}}
=\frac{\pi a}{18}
\left(\frac{\mu}{\mathcal R}\right)^4G^3M^2.
$$

Then $\beta_c\geq\beta^*$, or

$$
\boxed{1-\beta_c\leq1-\beta^*},
$$

and rearrangement gives exactly

$$
\boxed{M=\left(\frac6\pi\right)^{1/2}
\left[\left(\frac{\mathcal R}{\mu}\right)^4
\frac3a\,\frac{1-\beta^*}{\beta^{*4}}\right]^{1/2}
G^{-3/2}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
