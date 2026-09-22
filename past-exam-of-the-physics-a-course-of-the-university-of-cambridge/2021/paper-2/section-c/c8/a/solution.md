<h1 id="section-c/c8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The crystal has [periodic potential](../../../../../../periodic-potential.md) $V(x+a)=V(x)$. By [Bloch's theorem](../../../../../../bloch-s-theorem-split.md), an [energy eigenstate](../../../../../../energy-eigenstate.md) may be chosen as

$$
\psi_k(x)=e^{ikx}u_k(x),\qquad u_k(x+a)=u_k(x).
$$

Expand the periodic factor in a [Fourier series](../../../../../../fourier-series-split.md):

$$
u_k(x)=\sum_{n\in\mathbb Z}C_{k,n}e^{inG_1x},\qquad G_1=\frac{2\pi}{a}.
$$

Multiplication by $e^{ikx}$ gives the stated plane-wave expansion. Here $x$ is position, $a$ is the [primitive unit cell](../../../../../../primitive-unit-cell.md) length, $G_1$ is the primitive [reciprocal lattice](../../../../../../reciprocal-lattice.md) [wavenumber](../../../../../../wavenumber.md), $n$ runs over every integer, and $C_{k,n}$ are [complex numbers](../../../../../../complex-number.md) specifying the component [wave amplitudes](../../../../../../wave-amplitude.md). The [wavevector](../../../../../../wavevector.md) $k$ labels the [Bloch state](../../../../../../bloch-state.md) modulo $G_1$; $\hbar k$ is its [crystal momentum](../../../../../../crystal-momentum.md), rather than generally its measured free-space [momentum](../../../../../../momentum-split.md).

The component $e^{i(k+nG_1)x}$ is a [plane wave](../../../../../../plane-wave.md) of [wavevector](../../../../../../wavevector.md) $k+nG_1$. All these components acquire the same [phase factor](../../../../../../phase-factor.md) $e^{ika}$ under $x\mapsto x+a$, since $e^{inG_1a}=1$. Their mixing therefore respects the crystal's translation symmetry. The coefficients and [energy eigenvalue](../../../../../../energy-eigenvalue-split.md) follow from the [Schrödinger equation](../../../../../../schrodinger-equation.md); the expression is not a claim that the coefficients are equal or that only finitely many are nonzero. The [energy band](../../../../../../energy-band.md) index is suppressed in the notation, so different [energy bands](../../../../../../energy-band.md) at a common $k$ generally have different coefficient sets.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
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
