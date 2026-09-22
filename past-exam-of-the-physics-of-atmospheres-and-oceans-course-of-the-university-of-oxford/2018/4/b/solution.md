<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the large-[radius](../../../../radius.md) condensational-growth approximation from part (a), with fixed ambient [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) and transport resistances. It gives

$$
\frac{d(r^2)}{dt}=\frac{2(S-1)}{\rho(F_k^l+F_d^l)},\qquad
\boxed{t=\frac{\rho(F_k^l+F_d^l)(r^2-r_0^2)}{2(S-1)}.}
$$

Taking $\rho=10^3\,\mathrm{kg\,m^{-3}}$, $S-1=0.01$, and negligible initial $r_0^2$ gives

$$
\boxed{t_a\simeq202.5\,\mathrm s\simeq3.4\,\mathrm{min},\qquad
 t_b\simeq9.0\times10^5\,\mathrm s\simeq10.4\,\mathrm{days}.}
$$

The squared-[radius](../../../../radius.md) law makes [condensation](../../../../condensation.md) relatively fast for reaching [cloud](../../../../cloud.md)-droplet sizes but far too slow for producing millimetre rain within a typical evolving [cloud](../../../../cloud.md). Collision–coalescence, or ice growth followed by aggregation/riming and melting, bypasses this bottleneck. In reality [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) is shared by many particles and changes with ascent and vapour depletion, so even the constant-$1\%$ estimate is idealized.

These are growth times _after activation_, with negligible activation delay. The statement $r_0\ll1\,\mu\mathrm m$ alone does not ensure that a seed grows: for pure [water](../../../../water.md) with $B=0$, a seed with $r_0<A/(S-1)$ has a negative growth rate and shrinks. For soluble seeds the Köhler barrier depends on $A,B$ and the environmental [atmospheric supersaturation](../../../../atmospheric-supersaturation.md). The literal full-model time is

$$
t=\rho(F_k^l+F_d^l)\int_{r_0}^{r}\frac{r'\,dr'}{(S-1)-A/r'+B/r'^3},
$$

which cannot be assigned a unique initial-stage numerical value without those microphysical parameters. The two boxed estimates are the intended continuum [condensation](../../../../condensation.md) scales for activated droplets, rather than a claim that every arbitrarily small seed reaches those sizes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
