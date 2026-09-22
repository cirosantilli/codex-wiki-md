<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Follow a fluid element with position $\mathbf X(t)$ satisfying $\dot{\mathbf X}=\mathbf u(\mathbf X,t)$. The [chain rule](../../../../chain-rule.md) gives the [material derivative](../../../../material-derivative.md)

$$
\boxed{\frac{DQ}{Dt}=\frac d{dt}Q(\mathbf X(t),t)=\partial_tQ+\mathbf u\cdot\nabla Q.}
$$

Apply [Newton's second law](../../../../newton-s-second-law.md) to a material element of [volume](../../../../volume.md) $dV$ and [mass](../../../../mass.md) $\rho dV$. The net [pressure](../../../../pressure-split.md) [force](../../../../force-split.md) is $-\nabla p\,dV$, and [gravity](../../../../gravity.md) gives $-\rho\nabla\phi\,dV$. Dividing by the element [mass](../../../../mass.md), neglecting [viscosity](../../../../dynamic-viscosity-split.md) and using the [chain rule](../../../../chain-rule.md) componentwise gives the [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md)

$$
\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u=-\frac1\rho\nabla p-\nabla\phi.
$$

For a static spherical isothermal gas, $p=c_s^2\rho$ and $dp/dr=-GM(r)\rho/r^2$. Trial [density](../../../../density.md) $\rho=A/r^2$ gives enclosed [mass](../../../../mass.md) $M(r)=4\pi Ar$, so

$$
-\frac{2Ac_s^2}{r^3}=-\frac{4\pi GA^2}{r^3},\qquad
\boxed{A=\frac{c_s^2}{2\pi G}.}
$$

This is the [singular isothermal sphere](../../../../singular-isothermal-sphere.md). Its central [density](../../../../density.md) diverges, although the enclosed [mass](../../../../mass.md) tends to zero linearly and its total [mass](../../../../mass.md) inside a finite radius is finite. It is not the finite-central-density regular isothermal solution.

Truncate at $r_0$ with boundary [pressure](../../../../pressure-split.md) $p_0$. Then $M=4\pi Ar_0=2c_s^2r_0/G$ and $p_0=c_s^2\rho(r_0)$, giving

$$
\boxed{r_0=\frac{GM}{2c_s^2},\qquad p_0=\frac{c_s^4}{2\pi G r_0^2}.}
$$

The external medium is being treated as a prescribed [pressure](../../../../pressure-split.md) boundary; its own gravitational field is excluded from the cloud self-energy calculation.

For a monatomic [perfect gas](../../../../ideal-gas-split.md), the equilibrium is isothermal but the internal-energy relation still uses its [adiabatic index](../../../../heat-capacity-ratio.md) $\gamma=5/3$:

$$
U=\int\frac{p}{\gamma-1}\,dV=\frac32Mc_s^2.
$$

The gravitational self-energy follows by assembling shells:

$$
\Omega=-\int_0^{r_0}\frac{GM(r)}r\,dM(r)
=-16\pi^2GA^2r_0=-\frac{GM^2}{r_0}=-2Mc_s^2.
$$

Both [integrals](../../../../integral-split.md) remain finite at the singular center. Consequently

$$
\boxed{2U+\Omega=Mc_s^2=4\pi r_0^3p_0=3p_0\mathcal V,\qquad\mathcal V=4\pi r_0^3/3.}
$$

The [pressure-confined singular isothermal gas sphere](../../../../pressure-confined-singular-isothermal-gas-sphere.md) therefore satisfies the [virial theorem](../../../../virial-theorem.md) including the work of the confining surface [pressure](../../../../pressure-split.md). One can see its origin directly by integrating $\mathbf r\cdot\nabla p$: [integration by parts](../../../../integration-by-parts.md) gives $\oint p\,\mathbf r\cdot d\mathbf S-3\int p\,dV$, whose surface term is $4\pi r_0^3p_0$. An isolated vacuum-boundary version would omit that term and could not truncate this same positive-temperature isothermal profile at finite radius. The equality expresses equilibrium [force](../../../../force-split.md) and [energy](../../../../energy-split.md) balance, rather than proving [dynamical stability](../../../../stability-theory.md).

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
