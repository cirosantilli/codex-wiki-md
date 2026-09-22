<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

In [spherical coordinates](../../../../../spherical-coordinate-system.md), the angular [Laplacian](../../../../../laplacian.md) has [spherical harmonics](../../../../../spherical-harmonic.md) as [eigenfunctions](../../../../../eigenfunction.md), $L^2Y_{lm}=\hbar^2l(l+1)Y_{lm}$ and $L_zY_{lm}=\hbar mY_{lm}$. Separation leaves

$$
-\frac{\hbar^2}{2m}\left[R''+\frac2rR'-\frac{l(l+1)}{r^2}R\right]-\frac{C}{r}R=ER,
\qquad C=\frac{e^2}{4\pi\epsilon_0}.
$$

Regularity and normalizability give [principal quantum number](../../../../../principal-quantum-number.md) $n=1,2,\ldots$, orbital [quantum number](../../../../../quantum-number.md) $l=0,\ldots,n-1$, and [magnetic quantum number](../../../../../magnetic-quantum-number.md) $m=-l,\ldots,l$. Here the $m$ in the kinetic coefficient is the [electron mass](../../../../../electron-mass.md), distinct from the magnetic label.

For the proposed angular factor, $\cos\theta\propto Y_{10}$, so $l=1$ and [magnetic quantum number](../../../../../magnetic-quantum-number.md) zero. Direct differentiation gives $\nabla^2(re^{-\alpha r}\cos\theta)=(\alpha^2-4\alpha/r)\psi$. The $1/r$ term in the [Schrödinger equation](../../../../../schrodinger-equation.md) vanishes when $2\hbar^2\alpha/m=C$. With [Bohr radius](../../../../../bohr-radius.md) $a_0=\hbar^2/(mC)$,

$$
\boxed{\alpha=\frac1{2a_0},\qquad E=-\frac{\hbar^2\alpha^2}{2m}=-\frac{\hbar^2}{8ma_0^2}\simeq-3.40\,\mathrm{eV},\qquad l=1.}
$$

[wavefunction normalization](../../../../../wavefunction-normalization.md) uses $\int d\Omega\cos^2\theta=4\pi/3$ and $\int_0^\infty r^4e^{-2\alpha r}dr=24/(2\alpha)^5$, giving

$$
\boxed{A=\sqrt{\alpha^5/\pi}=\frac1{4\sqrt{2\pi}\,a_0^{5/2}}.}
$$

An arbitrary constant phase is allowed. This is the $2p_z$ state. Under spatial inversion, $r$ is unchanged and $\cos\theta$ changes sign, so its [parity](../../../../../parity.md) [eigenvalue](../../../../../eigenvalue.md) is **$-1$**, also given by $(-1)^l$.

Rotational invariance [means](../../../../../expected-value-split.md) rotated states have the same [energy](../../../../../energy-split.md); it does not require each member of a degenerate [energy](../../../../../energy-split.md) eigenspace to be invariant. [rotations](../../../../../rotation-mathematics.md) mix the three $l=1$ magnetic substates. An orbital oriented along $z$ can therefore have an anisotropic [probability density](../../../../../probability-density.md) while the [Hamiltonian](../../../../../hamiltonian.md) remains spherically symmetric.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
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
