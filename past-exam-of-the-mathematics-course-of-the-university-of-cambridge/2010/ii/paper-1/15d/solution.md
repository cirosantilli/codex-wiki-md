<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

Let the stellar radius be $R$ and assume zero external surface pressure. A spherical shell has mass $dm=4\pi r^2\rho\,dr$ and contributes $-Gm(r)\,dm/r$ to the [gravitational potential energy](../../../../../gravitational-energy.md). Using hydrostatic pressure support,

$$
E_{\rm grav}=-\int_0^R4\pi Gm\rho r\,dr
=4\pi\int_0^Rr^3P'\,dr
=-12\pi\int_0^Rr^2P\,dr
=\boxed{-3\langle P\rangle V}.
$$

The center boundary term vanishes and $P(R)=0$ eliminates the outer term. Nonzero external pressure would add $3P(R)V$.

The total energy is $(\alpha-3)\langle P\rangle V$, so energetic gravitational binding requires **$\alpha<3$**. For an isotropic gas, kinetic theory gives $P=(1/3)\int p v\,dn$. Nonrelativistic [kinetic energy](../../../../../kinetic-energy.md) is $pv/2$, giving $U=3PV/2$ and $\alpha=3/2$. Ultrarelativistic energy is $pv$, giving $U=3PV$ and $\alpha=3$: the ultrarelativistic limit is marginal in this Newtonian virial balance.

For a white dwarf, [electron degeneracy pressure](../../../../../electron-degeneracy-pressure.md) becomes ultrarelativistic as density increases. Its equation of state then scales as $P=K\rho^{4/3}$. Pressure support and gravitational stress have the same radius scaling, leaving a limiting mass of order $(K/G)^{3/2}$ rather than allowing arbitrary mass to be supported by contraction. The [Chandrasekhar limit](../../../../../chandrasekhar-limit.md) is this maximum mass for a cold electron-degenerate star at specified composition, of order $(\hbar c/G)^{3/2}/(\mu_e m_p)^2$.

The virial calculation by itself does not establish a universal numerical maximum mass for every stellar composition and equation of state; its precise consequence is loss of binding/support as the pressure-bearing particles become ultrarelativistic. An accreting carbon-oxygen white dwarf approaching its limiting mass typically undergoes runaway carbon burning and thermonuclear disruption, a [Type Ia supernova](../../../../../type-ia-supernova.md). For other compositions or evolution, electron captures can instead lead to collapse into a neutron star. The subsequent evolution needs that physical distinction.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
