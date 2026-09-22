<h1 id="20a/solution">Solution</h1>

↑ **Parent:** [20A](../20a.md)

The time-independent [Schrödinger equation](../../../../../schrodinger-equation.md) is $[-\hbar^2\nabla^2/(2m)+V]\psi=E\psi$, with attractive [Coulomb potential](../../../../../coulomb-potential-energy.md) $V(r)=-\kappa/r$, where $\kappa=e^2/(4\pi\varepsilon_0)$. Separating $\psi=R(r)Y_\ell^m(\theta,\varphi)$ uses the [spherical harmonic](../../../../../spherical-harmonic.md) angular [eigenvalue](../../../../../eigenvalue.md) $-\ell(\ell+1)$ of the unit-sphere [Laplacian](../../../../../laplacian.md). The radial kinetic contribution is $-\hbar^2(R''+2R'/r)/(2m)$, the angular kinetic contribution is the centrifugal term $\hbar^2\ell(\ell+1)R/(2mr^2)$, and the remaining term is the attractive [potential energy](../../../../../potential-energy.md). The right side is the [energy eigenvalue](../../../../../energy-eigenvalue.md) times the radial [wavefunction](../../../../../wave-function.md). Here the stated $m$ neglects nuclear recoil; including it replaces the electron mass by the [reduced mass](../../../../../reduced-mass.md).

For $\ell=0$, substitution of the ground-state exponential gives

$$
-\frac{\hbar^2}{2m}(\alpha^2-2\alpha/r)-\frac\kappa r=E_1.
$$

Its $1/r$ coefficient must vanish and its constant coefficient determines the [energy](../../../../../energy.md), so

$$
\boxed{\alpha=\frac{m\kappa}{\hbar^2}=\frac1{a_0},\qquad E_1=-\frac{m\kappa^2}{2\hbar^2}.}
$$

Here $a_0=\hbar^2/(m\kappa)$ is the [Bohr radius](../../../../../bohr-radius.md).

For $R_2=N_2(r+b)e^{-\beta r}$, direct differentiation yields

$$
R_2''+\frac2rR_2'=N_2e^{-\beta r}\left[\beta^2(r+b)-4\beta+\frac{2-2\beta b}{r}\right].
$$

Cancel the nonzero exponential in the radial [Schrödinger equation](../../../../../schrodinger-equation.md) and compare coefficients of $r$, the constant term, and $1/r$. They give, respectively,

$$
E_2=-\frac{\hbar^2\beta^2}{2m},\qquad \frac{2\hbar^2\beta}{m}=\kappa,\qquad \frac{\hbar^2}{m}(\beta b-1)-\kappa b=0.
$$

Consequently

$$
\boxed{\beta=\frac1{2a_0},\qquad b=-2a_0,\qquad E_2=-\frac{m\kappa^2}{8\hbar^2}=\frac14E_1.}
$$

The positive decay constants ensure normalizability; the second radial [wavefunction](../../../../../wave-function.md) has one positive-radius node at $2a_0$, as appropriate to the first radial excitation.

If the entire energy gap is carried by one [photon](../../../../../photon.md), neglecting atomic recoil, [conservation of energy](../../../../../conservation-of-energy.md) gives the requested frequency

$$
\boxed{\nu_{\rm gap}=\frac{E_2-E_1}{h}=\frac{3m\kappa^2}{8h\hbar^2}=\frac{3me^4}{8h\hbar^2(4\pi\varepsilon_0)^2}.}
$$

There is a physical qualification: these are the $2s$ and $1s$ states, so the usual single-photon electric-dipole transition is forbidden by the [electric-dipole selection rules for hydrogen](../../../../../electric-dipole-selection-rules-for-hydrogen.md). Explicitly, both angular factors are $Y_0^0$, and $\int |Y_0^0|^2\hat{\mathbf r}\,d\Omega=0$, so every component of $\langle1s|\mathbf r|2s\rangle$ vanishes. The leading isolated-atom decay is instead two-photon emission, for which $\nu_1+\nu_2=\nu_{\rm gap}$ and individual frequencies are not fixed. This metastability and the two-photon channel are documented in [NIST's hydrogen spectral-data compilation](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=842564). Thus the boxed answer is the energy-gap frequency under the printed single-photon assumption, rather than an assertion of an allowed electric-dipole line.

## ↑ Ancestors (10)

1. [20A](../20a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
