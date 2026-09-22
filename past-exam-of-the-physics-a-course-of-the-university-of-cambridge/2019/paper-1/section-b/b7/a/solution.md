<h1 id="section-b/b7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the nonrelativistic [Coulomb potential energy](../../../../../../coulomb-potential-energy.md) $V=-Ze^2/(4\pi\epsilon_0r)$, with the nucleus treated as fixed. Since the [wavefunction](../../../../../../wave-function-split.md) has zero [orbital angular momentum](../../../../../../orbital-angular-momentum.md), its [Laplacian](../../../../../../laplacian.md) is

$$
\nabla^2\psi=\frac1{r^2}\frac{d}{dr}\left(r^2\frac{d\psi}{dr}\right)=\left(\beta^2-\frac{2\beta}{r}\right)\psi.
$$

Substituting into the time-independent [Schrödinger equation](../../../../../../schrodinger-equation.md) gives

$$
\frac{H\psi}{\psi}=-\frac{\hbar^2\beta^2}{2m_e}+\frac1r\left(\frac{\hbar^2\beta}{m_e}-\frac{Ze^2}{4\pi\epsilon_0}\right).
$$

For a constant [energy eigenvalue](../../../../../../energy-eigenvalue-split.md), the coefficient of $1/r$ must vanish. Therefore $\boxed{\beta=Z/a_0}$, where $a_0$ is the [Bohr radius](../../../../../../bohr-radius.md). [Wavefunction normalization](../../../../../../wavefunction-normalization.md) then requires

$$
1=4\pi|\alpha|^2\int_0^\infty r^2e^{-2\beta r}\,dr=\frac{\pi|\alpha|^2}{\beta^3}.
$$

Choosing the irrelevant overall phase so that $\alpha$ is real and positive gives $\boxed{\alpha^2=\beta^3/\pi}$. The remaining constant term is the [hydrogen ground-state energy](../../../../../../hydrogen-ground-state-energy.md)

$$
\boxed{E=-\frac{\hbar^2\beta^2}{2m_e}=-\frac{m_eZ^2e^4}{2(4\pi\epsilon_0)^2\hbar^2}\simeq-13.6Z^2\,\mathrm{eV}.}
$$

Replacing $m_e$ by the electron-nucleus [reduced mass](../../../../../../reduced-mass.md) gives the usual finite-nuclear-mass refinement.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
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
