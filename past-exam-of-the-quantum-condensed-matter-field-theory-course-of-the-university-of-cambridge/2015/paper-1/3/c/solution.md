<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the physical density-phase contour put $\bar\psi=\sqrt\rho\,e^{-i\phi}$. Direct differentiation gives

$$
\bar\psi\partial_\tau\psi=\frac12\partial_\tau\rho+i\rho\partial_\tau\phi,
\qquad
|\nabla\psi|^2=\frac{|\nabla\rho|^2}{4\rho}+\rho|\nabla\phi|^2.
$$

Integrating the [Laplacian](../../../../../laplacian.md) by parts with the stated bulk boundary convention, and dropping the periodic total [derivative](../../../../../derivative.md) of $\rho$, produces the [density-phase action of a Bose gas](../../../../../density-phase-action-of-a-bose-gas.md),

$$
S=\int d\tau\,d^dr\left[i\rho\partial_\tau\phi
+\frac{|\nabla\rho|^2}{8m\rho}+\frac\rho{2m}|\nabla\phi|^2
+\frac g2(\rho-\rho_0)^2-\frac{\mu^2}{2g}\right].
$$

Write $\rho=\rho_0+\delta\rho$ and $\phi=\phi_0+\varphi$, where $\phi_0$ is constant. To quadratic order,

$$
\boxed{S_2=\int d\tau\,d^dr\left[
\frac g2(\delta\rho)^2+i\delta\rho\partial_\tau\varphi
+\frac{|\nabla\delta\rho|^2}{8m\rho_0}
+\frac{\rho_0}{2m}|\nabla\varphi|^2\right].}
$$

The uniform static density fluctuation has positive curvature $g$. Its inverse static susceptibility at [wavevector](../../../../../wavevector.md) $q$ is $A_q=g+q^2/(4m\rho_0)$, which remains nonzero at $q=0$. This is the sense in which the amplitude or density fluctuation is massive. The phase has no term proportional to $\varphi^2$ without [derivatives](../../../../../derivative.md); a uniform phase [rotation](../../../../../rotation-mathematics.md) costs no [action](../../../../../action.md). It is the massless direction required by global $U(1)$ [symmetry](../../../../../symmetry-physics.md).

The term $i\delta\rho\partial_\tau\varphi$ shows [density-phase conjugacy](../../../../../density-phase-conjugacy.md). It is important to distinguish [static density stiffness versus an excitation gap](../../../../../static-density-stiffness-versus-an-excitation-gap.md): the density and phase do not form two independent normal-mode branches with one gapped and one gapless particle. In this nonrelativistic first-order theory they supply the conjugate variables of one positive Bogoliubov branch, derived below. The omitted cubic terms include $\delta\rho|\nabla\varphi|^2/(2m)$ and corrections from the density-gradient denominator.

There is also a background term $i\rho_0\int d\tau\,d^dr\,\partial_\tau\varphi$. It vanishes for smooth fluctuations with zero temporal winding. Periodicity of $\psi$, however, permits $\varphi(\beta)-\varphi(0)=2\pi w$. The [compact phase winding term](../../../../../compact-phase-winding-term.md) must be retained when such sectors are included; it is not generally the same constant in all sectors. The local Gaussian [phonon](../../../../../phonon.md) calculation concerns the smooth zero-winding sector and does not describe vortices or points where the density vanishes.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
