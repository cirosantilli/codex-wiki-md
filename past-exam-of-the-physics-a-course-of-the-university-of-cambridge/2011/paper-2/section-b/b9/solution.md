<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

Put $\kappa=e^2/(4\pi\epsilon_0)$. Substitution of $\psi=R(r)\Phi(\phi)$ into the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md), followed by division by $R\Phi$ and multiplication by $r^2$, separates the angular dependence:

$$
\frac{r^2R''+rR'}R+\frac{2\mu}{\hbar^2}(Er^2+\kappa r)
=-\frac{\Phi''}{\Phi}=m^2.
$$

Thus $\Phi=e^{im\phi}/\sqrt{2\pi}$ and

$$
rR''+R'+\left[\frac{2\mu}{\hbar^2}(Er+\kappa)-\frac{m^2}{r}\right]R=0.
$$

The [single-valued wavefunction](../../../../../single-valued-wavefunction.md) condition, $\Phi(\phi+2\pi)=\Phi(\phi)$, requires **$m\in\mathbb Z$**. The regular [boundary condition](../../../../../boundary-condition.md) at the origin selects $R\sim r^{|m|}$. Accordingly use $s=|m|$ in the radial ansatz; the printed $x^m$ notation describes the $m\geq0$ representatives.

For the [two-dimensional Coulomb bound state](../../../../../two-dimensional-coulomb-bound-state.md), substitution of $R=x^s e^{-x/2}G$ with the stipulated radial and [energy](../../../../../energy-split.md) scales gives

$$
xG''+(2s+1-x)G'+(N-s-\tfrac12)G=0.
$$

The coefficient of $x^n$ in the [power series](../../../../../power-series.md) is

$$
(n+1)(n+2s+1)a_{n+1}
+(N-s-\tfrac12-n)a_n=0,
\qquad
\boxed{a_{n+1}=\frac{n+s+\tfrac12-N}{(n+1)(n+2s+1)}a_n}.
$$

The regular solution otherwise has an exponentially growing contribution at large $x$, incompatible with being [normalizable](../../../../../normalizable-wavefunction.md). Termination at degree $n_r\geq0$ therefore requires

$$
\boxed{N=n_r+|m|+\tfrac12,\quad
E_{n_rm}=-\frac{\mu\kappa^2}{2\hbar^2(n_r+|m|+\tfrac12)^2}}.
$$

The resulting $G$ is proportional to a [Generalized Laguerre polynomial](../../../../../generalized-laguerre-polynomial.md).

Define $R_{\rm y}=\mu\kappa^2/(2\hbar^2)$, the hydrogenic Rydberg [energy](../../../../../energy-split.md) for the stipulated [mass](../../../../../mass.md). The first three distinct two-dimensional [energies](../../../../../energy-split.md) are **$-4R_{\rm y},-4R_{\rm y}/9,-4R_{\rm y}/25$**, whereas in three dimensions they are **$-R_{\rm y},-R_{\rm y}/4,-R_{\rm y}/9$**. Both series approach zero from below, but the planar [ground state](../../../../../ground-state.md) is four times more tightly bound. Without [spin](../../../../../spin.md) the respective [quantum degeneracies](../../../../../degenerate-energy-levels.md) are $1,3,5$ and $1,4,9$; if individual degenerate states are counted, the second and third planar states already share the first excited [energy](../../../../../energy-split.md). This comparison retains the supplied $1/r$ interaction; it does not replace it by the logarithmic [electrostatic potential](../../../../../electric-potential.md) of a genuinely two-dimensional electromagnetic theory.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
