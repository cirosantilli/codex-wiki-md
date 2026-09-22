<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $N=300$, the critical [polymer](../../../../../polymer-split.md) [volume fraction](../../../../../volume-fraction.md) is

$$
\phi_c=\frac1{1+\sqrt{300}}\simeq0.05458.
$$

If $v_0$ is the volume assigned to one [amino acid](../../../../../amino-acid.md) in the lattice model, the critical [number densities](../../../../../number-density.md) are exactly

$$
\boxed{n_{m,c}=\frac{\phi_c}{v_0},\qquad
n_{p,c}=\frac{\phi_c}{Nv_0}=\frac{n_{m,c}}{300}.}
$$

The extra physical approximation needed to use the given [radius of gyration](../../../../../radius-of-gyration.md) is that a chain in a [poor solvent](../../../../../poor-solvent.md) is a compact [polymer globule](../../../../../polymer-globule.md). Its size then scales as $R_g\sim bN^{1/3}$ with $v_0\sim b^3$, so $Nv_0\sim R_g^3$. This gives the standard scaling estimates

$$
n_{m,c}\sim\frac{N\phi_c}{R_g^3},\qquad
n_{p,c}\sim\frac{\phi_c}{R_g^3}.
$$

With $R_g=3\,\mathrm{nm}$, numerical substitution gives

$$
\boxed{n_{m,c}\sim6\times10^{26}\,\mathrm{m^{-3}},\qquad
n_{p,c}\sim2\times10^{24}\,\mathrm{m^{-3}}.}
$$

Using only the leading large-$N$ value $\phi_c\sim N^{-1/2}$ gives $6.4\times10^{26}$ and $2.1\times10^{24}\,\mathrm{m^{-3}}$, respectively. These are scaling estimates, not geometrically exact densities.

For comparison, a specifically _uniform spherical_ compact protein has the [radius of gyration of a uniform sphere](../../../../../radius-of-gyration-of-a-uniform-sphere.md), $R_g^2=3R^2/5$, so its physical volume is $V_p=(4\pi/3)(5/3)^{3/2}R_g^3$. Taking $Nv_0=V_p$ instead gives $n_{m,c}\simeq6.7\times10^{25}\,\mathrm{m^{-3}}$ and $n_{p,c}\simeq2.2\times10^{23}\,\mathrm{m^{-3}}$. The factor between these conventions is geometric. The PDF does not give a [monomer](../../../../../monomer.md) volume, globule density or shape model, and a [radius of gyration](../../../../../radius-of-gyration.md) alone does not determine an exact molecular volume. The model-independent conclusions are the formulas in terms of $v_0$ and the 300:1 ratio of [monomer](../../../../../monomer.md) to protein number density.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
