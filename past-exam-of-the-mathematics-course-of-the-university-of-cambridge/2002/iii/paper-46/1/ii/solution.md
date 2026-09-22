<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $M_*$ be the central [mass](../../../../../../mass.md), so $\Omega^2=GM_*/r^3$ and the [specific orbital energy](../../../../../../specific-orbital-energy.md) is $\varepsilon=-GM_*/(2r)$. Define the inward [accretion rate](../../../../../../accretion-rate.md) $\dot M>0$. The rate at which the gas acquires binding [energy](../../../../../../energy.md) in moving from $b$ to $a$ is

$$
\boxed{B_{a,b}=\dot M\{\varepsilon(b)-\varepsilon(a)\}=\frac{GM_*\dot M}{2}\left(\frac1a-\frac1b\right).}
$$

The vertically integrated viscous heating per unit horizontal area, including the entire column, is $\bar\nu\Sigma(r\Omega')^2$. Since $r\Omega'=-3\Omega/2$, the dissipated power in the annulus is

$$
D_{a,b}=\int_a^b2\pi r\,\bar\nu\Sigma\frac94\Omega^2\,dr=\frac{3GM_*\dot M}{2}\int_a^b\frac1{r^2}\left(1-\sqrt{\frac{r_{\rm in}}r}\right)dr.
$$

Here the column [integral](../../../../../../integral.md) already includes dissipation associated with both disk faces; adding another factor of two would double-count it. Performing the elementary [integrals](../../../../../../integral.md) gives

$$
\boxed{D_{a,b}=GM_*\dot M\left[\frac32\left(\frac1a-\frac1b\right)-\sqrt{r_{\rm in}}\left(a^{-3/2}-b^{-3/2}\right)\right].}
$$

For the whole disk, take $a=r_{\rm in}$ and $b\to\infty$. Both expressions give

$$
\boxed{D_{\rm disk}=B_{\rm disk}=\frac{GM_*\dot M}{2r_{\rm in}}.}
$$

If $a\gg r_{\rm in}$, the bracket $1-\sqrt{r_{\rm in}/r}$ is uniformly close to one throughout the annulus. Comparing the positive [integrals](../../../../../../integral.md) shows

$$
\frac{D_{a,b}}{B_{a,b}}=3\left[1+O\left(\sqrt{\frac{r_{\rm in}}a}\right)\right],
$$

with the correction negative. Thus **far from the inner edge the [viscous dissipation](../../../../../../viscous-dissipation.md) is approximately three times the local binding-energy acquisition**.

There is no violation of [conservation of energy](../../../../../../conservation-of-energy.md) because the [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) also transports mechanical [energy](../../../../../../energy.md). The outward [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) is

$$
\mathcal G=-2\pi\bar\nu\Sigma r^3\Omega'=\dot M\big(\sqrt{GM_*r}-\sqrt{GM_*r_{\rm in}}\big),
$$

and its outward [energy](../../../../../../energy.md) flux is $\Omega\mathcal G=GM_*\dot M[r^{-1}-\sqrt{r_{\rm in}}r^{-3/2}]$. The explicit expressions satisfy

$$
\boxed{D_{a,b}=B_{a,b}+\Omega(a)\mathcal G(a)-\Omega(b)\mathcal G(b).}
$$

[Energy](../../../../../../energy.md) transported from the inner disk supplies the extra dissipation at larger radii. The torque power vanishes at the [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md) and tends to zero at infinity, leaving global balance. This is [torque transport of energy in a steady accretion disk](../../../../../../torque-transport-of-energy-in-a-steady-accretion-disk.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
