<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), total upper-layer [kinetic energy](../../../../../../kinetic-energy.md) is $K=\rho_lShu_U^2/2$, where $u_U$ is its volume root-mean-square speed. For [solid-body rotation](../../../../../../solid-body-rotation.md) of angular speed $\omega(t)$, direct radial averaging gives $u_U^2=\omega^2R^2/2$, consistent with that energy expression. A constant $K$ implies $hu_U^2=h_0u_U(0)^2$. Define $C_K=u_U(0)/(\Omega R)$ to obtain the [fixed-energy turbulent mixed layer](../../../../../../fixed-energy-turbulent-mixed-layer.md) relation

$$
\boxed{hu_U^2=C_K^2\Omega^2R^2h_0.}
$$

With $u_I=C_Iu_U$, the [interfacial power model for entrainment](../../../../../../interfacial-power-model-for-entrainment.md) used in (b) gives

$$
\dot h=\frac{2C_Wc_DC_I^3C_K^3\Omega^3R^3}{B}
\left(\frac{h_0}{h}\right)^{3/2}.
$$

Multiply by $h^{3/2}$ and integrate from $h_0$. This yields

$$
h^{5/2}=h_0^{5/2}
+\frac{5C_Wc_DC_I^3C_K^3\Omega^3R^3h_0^{3/2}}B\,t.
$$

The [fixed-energy two-layer entrainment law](../../../../../../fixed-energy-two-layer-entrainment-law.md) is therefore

$$
\boxed{\frac h{h_0}=(1+A\Omega t)^{2/5},\qquad
A=\frac{5C_Wc_DC_I^3C_K^3\Omega^2R^3}{Bh_0}
=\frac{5C_Wc_DC_I^3C_K^3}{\mathrm{Ri}_{B,0}}\frac R{h_0}.}
$$

Here $\mathrm{Ri}_{B,0}=B/(\Omega^2R^2)$ uses the same lid-speed normalization as part (b). All numerical geometry factors depend on the chosen characteristic stress/speed convention. The formula ceases to apply once $h=H$.

The exponent $2/5$ requires the local power to decrease as $u_I^3\propto h^{-3/2}$. It does not follow from constant upper-layer [kinetic energy](../../../../../../kinetic-energy.md) and a fixed fraction of unspecified lid power alone. For example, an imposed constant shaft power together with a constant fraction going to [potential energy](../../../../../../potential-energy.md) would give constant $\dot h$, not this exponent. The appropriate distinction between local interface power and global forcing appears explicitly in the primary study [Entrainment and mixed layer dynamics of a surface-stress-driven stratified fluid](https://www.whoi.edu/cms/files/entrainment_mixedlayer_201804.pdf), equations (3.6)–(3.7); the calculations above use that local interpretation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
