<h1 id="section-b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\varepsilon=\varepsilon_0\varepsilon_r$ be the [permittivity](../../../../../permittivity-split.md), $\beta=(k_BT)^{-1}$, $e>0$ the [elementary charge](../../../../../elementary-charge.md), and $c$ the bulk salt formula-unit [number density](../../../../../number-density.md). The [Boltzmann distribution](../../../../../boltzmann-distribution.md) gives

$$
n_{\mathrm{Mg}}(r)=c\,e^{-2\beta e\phi(r)},\qquad
n_{\mathrm{Cl}}(r)=2c\,e^{\beta e\phi(r)}.
$$

Consequently the exterior [Poisson-Boltzmann equation](../../../../../poisson-boltzmann-equation.md) is

$$
\frac1{r^2}\frac d{dr}\left(r^2\frac{d\phi}{dr}\right)
=-\frac{2ec}{\varepsilon}\left(e^{-2\beta e\phi}-e^{\beta e\phi}\right),\qquad r>a.
$$

For small $Q$, meaning $2\beta e|\phi(a)|\ll1$, linearize the exponentials. The [Debye–Hückel approximation](../../../../../debye-huckel-approximation.md) gives

$$
\rho_{\mathrm{ion}}\simeq-6\beta e^2c\phi,\qquad
\frac1{r^2}(r^2\phi')'=\kappa^2\phi,\qquad
\boxed{\kappa^2=\frac{6e^2c}{\varepsilon k_BT},\quad \lambda_D=\kappa^{-1}.}
$$

This is also $\kappa^2=\beta e^2\sum_i z_i^2 n_{i,\infty}/\varepsilon$: the divalent cation contributes $4c$ and the two monovalent anions contribute $2c$. In terms of molar salt concentration $C$ in $\mathrm{mol\,m^{-3}}$, replace $c$ by $N_A C$; if $C$ is in $\mathrm{mol\,L^{-1}}$, use $c=10^3N_A C$. The molar [ionic strength](../../../../../ionic-strength.md) is $3C$ in the same concentration units.

The boundary conditions are $\phi(\infty)=0$ and, by [Gauss's law](../../../../../gauss-s-law.md),

$$
-\varepsilon\phi'(a^+)=\frac{Q}{4\pi a^2}.
$$

Here the surface charge is uniform and the spherically symmetric interior field is zero. Set $u=r\phi$; the radial equation reduces to $u''=\kappa^2u$. Decay excludes the growing exponential, so write $\phi=B e^{-\kappa(r-a)}/r$. Then $\phi'(a)=-B(1+\kappa a)/a^2$, giving

$$
\boxed{\phi(r)=\frac{Q}{4\pi\varepsilon\,r(1+\kappa a)}e^{-\kappa(r-a)}.}
$$

It solves the _linearized_ [Poisson-Boltzmann equation](../../../../../poisson-boltzmann-equation.md), not the full nonlinear equation at finite $Q$. The radial ion profiles, consistently to first order, are

$$
\boxed{n_{\mathrm{Mg}}(r)\simeq c[1-2\beta e\phi(r)],\qquad
n_{\mathrm{Cl}}(r)\simeq2c[1+\beta e\phi(r)].}
$$

The exponential [Boltzmann distribution](../../../../../boltzmann-distribution.md) formulas above express the full mean-field relation, but substituting a linearized potential into them is accurate only to the retained order. A useful [electroneutrality](../../../../../electroneutrality.md) check is

$$
4\pi\int_a^\infty\rho_{\mathrm{ion}}r^2dr
=-4\pi\varepsilon[r^2\phi']_a^\infty=-Q.
$$

The result is the [Debye-Hückel potential of a charged sphere](../../../../../debye-huckel-potential-of-a-charged-sphere.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
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
