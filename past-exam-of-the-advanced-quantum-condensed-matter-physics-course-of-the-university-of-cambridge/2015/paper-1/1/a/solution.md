<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use normalized plane-wave [spin](../../../../../spin.md) orbitals $V^{-1/2}e^{i\mathbf k\cdot\mathbf r}\chi_\sigma$ and fill a separate [Fermi sphere](../../../../../fermi-sphere.md) for each [spin](../../../../../spin.md) species. Each [spin](../../../../../spin.md) state counts once, so

$$
n_\sigma=\int_{|\mathbf k|<k_{F\sigma}}\frac{d^3k}{(2\pi)^3}
=\frac{k_{F\sigma}^3}{6\pi^2}.
$$

Its [kinetic energy](../../../../../kinetic-energy.md) per [volume](../../../../../volume.md) is

$$
\frac{T_\sigma}{V}=\int_{|\mathbf k|<k_{F\sigma}}\frac{d^3k}{(2\pi)^3}
\frac{\hbar^2k^2}{2m_e}
=\frac{\hbar^2 k_{F\sigma}^5}{20\pi^2m_e}
=A n_\sigma^{5/3},
\qquad
\boxed{A=\frac{3\hbar^2}{10m_e}(6\pi^2)^{2/3}.}
$$

The spin-independent contact interaction has uncancelled direct [energy](../../../../../energy-split.md) $E_H/V=\gamma n^2/2$, with $n=n_\uparrow+n_\downarrow$. By the imposed background assumption this direct contribution cancels. For the Fock term the contact delta function sets the two spatial positions equal; its [spin](../../../../../spin.md) factors then select equal spins. The local one-body [density](../../../../../density.md) matrix for each [spin](../../../../../spin.md) has diagonal value $n_\sigma$, giving

$$
\frac{E_X}{V}=-\frac\gamma2\sum_\sigma n_\sigma^2.
$$

Combining these results gives the [contact-interaction Hartree-Fock spin energy](../../../../../contact-interaction-hartree-fock-spin-energy.md)

$$
\boxed{\frac{E_0}{V}=A(n_\uparrow^{5/3}+n_\downarrow^{5/3})
-\frac\gamma2(n_\uparrow^2+n_\downarrow^2).}
$$

Here $\gamma$ has units of [energy](../../../../../energy-split.md) times [volume](../../../../../volume.md). The result is the model with the stated background subtraction; an isolated contact-interacting gas without that subtraction retains its direct contribution.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Condensed Matter Physics course of the University of Cambridge](../../../../../advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
