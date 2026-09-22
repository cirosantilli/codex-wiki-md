<h1 id="section-b/b6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The attractive [Coulomb potential energy](../../../../../../coulomb-potential-energy.md) is $V(r)=-e^2/(4\pi\epsilon_0r)$, so

$$
\frac1r\frac{dV}{dr}=\frac{e^2}{4\pi\epsilon_0r^3}.
$$

Use precisely the radial normalization stated in the PDF: the radial probability measure is $4\pi r^2|\psi|^2dr$. The supplied function has

$$
|\psi|^2=\frac{r^2}{96\pi a_0^5}e^{-r/a_0},
\qquad4\pi r^2|\psi|^2dr=\frac{r^4e^{-r/a_0}}{24a_0^5}dr.
$$

Its integral is one, since $\int_0^\infty r^4e^{-r/a_0}dr=24a_0^5$. In particular,

$$
\langle r^{-3}\rangle=\frac1{24a_0^5}\int_0^\infty re^{-r/a_0}dr
=\frac1{24a_0^3}.
$$

This calculation uses the supplied convention, rather than multiplying a separately normalized standard radial function by an extra $4\pi$.

The [addition of angular momentum](../../../../../../addition-of-angular-momentum.md) bracket is $j(j+1)-l(l+1)-s(s+1)=3/4-2-3/4=-2$. Substitution in the [spin-orbit energy shift in a central potential](../../../../../../spin-orbit-energy-shift-in-a-central-potential.md) therefore gives

$$
\boxed{\langle H_1\rangle
=-\frac{\hbar^2}{2m^2c^2}\frac{e^2}{4\pi\epsilon_0}\frac1{24a_0^3}
=-\frac{\hbar^2e^2}{192\pi\epsilon_0m^2c^2a_0^3}
\simeq-3.02\times10^{-5}\,\mathrm{eV}.}
$$

Here $a_0=5.29\times10^{-11}\,\mathrm m$ is the supplied [Bohr radius](../../../../../../bohr-radius.md). The negative sign means the $j=1/2$ member of the $l=1$ pair is shifted downward by this [spin-orbit interaction](../../../../../../spin-orbit-interaction.md); it is not the total hydrogen binding energy.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
