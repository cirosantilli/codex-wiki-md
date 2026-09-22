<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

The [Time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is $[-\hbar^2\nabla^2/(2m)+V]\Psi=E\Psi$. For the [hydrogen atom](../../../../../hydrogen-atom.md), separate variables as $\Psi=g(r)Y_{\ell m}(\theta,\varphi)$. The spherical-coordinate [Laplacian](../../../../../laplacian.md) has radial part $r^{-2}\partial_r(r^2\partial_r)$ and angular part $r^{-2}\Delta_{S^2}$. A [spherical harmonic](../../../../../spherical-harmonic.md) obeys $\Delta_{S^2}Y_{\ell m}=-\ell(\ell+1)Y_{\ell m}$. The first displayed term is therefore radial kinetic energy; the second is the attractive [Coulomb's law](../../../../../coulomb-s-law.md) potential energy $-e^2/(4\pi\varepsilon_0r)$ of electron and proton; the third is the angular kinetic energy, also called the [centrifugal potential](../../../../../centrifugal-potential.md). Regular single-valued angular states have $\boxed{\ell=0,1,2,\ldots}$, with [orbital angular momentum](../../../../../orbital-angular-momentum.md) squared $\hbar^2\ell(\ell+1)$.

For $g=r^\alpha e^{-\beta r}$, direct differentiation gives

$$
\frac{g''+2g'/r}{g}=\frac{\alpha(\alpha+1)}{r^2}-\frac{2\beta(\alpha+1)}r+\beta^2.
$$

Substitution into the [Radial Schrodinger equation for the hydrogen atom](../../../../../radial-schrodinger-equation-for-the-hydrogen-atom.md) and equality of the coefficients of $r^{-2}$, $r^{-1}$ and the constant term give

$$
\alpha(\alpha+1)=\ell(\ell+1),\qquad \frac{\hbar^2\beta(\alpha+1)}m=\frac{e^2}{4\pi\varepsilon_0},\qquad E=-\frac{\hbar^2\beta^2}{2m}.
$$

The regular radial solution selects $\alpha=\ell$, rather than the singular branch $-\ell-1$. At $\ell=0$, $r^{-1}$ is locally square integrable but is still inadmissible as a regular Coulomb eigenfunction: its [Laplacian](../../../../../laplacian.md) has a point-source contribution at the origin. Bound-state decay requires $\beta>0$. Thus, with the [Bohr radius](../../../../../bohr-radius.md) $a_0=4\pi\varepsilon_0\hbar^2/(me^2)$,

$$
\boxed{\alpha=\ell,\qquad\beta=\frac1{a_0(\ell+1)},\qquad E_\ell=-\frac{me^4}{2(4\pi\varepsilon_0)^2\hbar^2(\ell+1)^2}.}
$$

These are the nodeless states with [principal quantum number](../../../../../principal-quantum-number.md) $n=\ell+1$. Increasing $\ell$ raises the energy towards zero, so emission is from the state labelled $\ell+1$ to the one labelled $\ell$. Using the [Planck constant](../../../../../planck-constant.md) $h=2\pi\hbar$ and [photon](../../../../../photon.md) energy $h\nu$, the frequency is

$$
\boxed{\nu=\frac{me^4}{2(4\pi\varepsilon_0)^2\hbar^2h}\left[\frac1{(\ell+1)^2}-\frac1{(\ell+2)^2}\right].}
$$

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
