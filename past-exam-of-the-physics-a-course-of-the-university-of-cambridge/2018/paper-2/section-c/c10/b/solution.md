<h1 id="section-c/c10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Impose periodic [boundary conditions](../../../../../../boundary-condition.md) on a large cubic box. The allowed [wavevectors](../../../../../../wavevector.md) occupy a lattice of cell volume $(2\pi)^3/V$ in [wavevector](../../../../../../wavevector.md) space. Including the two spin states, the number of states with magnitude at most $k$ is

$$
\mathcal N(k)=2\frac{V}{(2\pi)^3}\frac{4\pi k^3}{3}=\frac{Vk^3}{3\pi^2}.
$$

Using $k=\sqrt{2m_e\epsilon}/\hbar$ and differentiating gives the total, spin-summed [three-dimensional free-electron density of states](../../../../../../three-dimensional-free-electron-density-of-states.md),

$$
\boxed{g(\epsilon)=\frac{V}{2\pi^2}\left(\frac{2m_e}{\hbar^2}\right)^{3/2}\sqrt\epsilon},\qquad \epsilon\geq0.
$$

It counts states per unit [energy](../../../../../../energy-split.md); divide by $V$ for states per unit [volume](../../../../../../volume.md) per unit [energy](../../../../../../energy-split.md). At zero [temperature](../../../../../../temperature-split.md), the [Fermi-Dirac distribution](../../../../../../fermi-dirac-distribution.md) fills all states up to the [Fermi energy](../../../../../../fermi-energy.md), giving

$$
N=\int_0^{E_F}g(\epsilon)\,d\epsilon
=\frac{V}{3\pi^2}\left(\frac{2m_eE_F}{\hbar^2}\right)^{3/2}.
$$

Writing $n=N/V$ gives

$$
\boxed{k_F=(3\pi^2n)^{1/3}},\qquad
\boxed{E_F=\frac{\hbar^2}{2m_e}(3\pi^2n)^{2/3}},\qquad
\boxed{g(E_F)=\frac{3N}{2E_F}}.
$$

The [energy](../../../../../../energy-split.md) zero is the bottom of the free-electron band. The [electron Fermi temperature](../../../../../../electron-fermi-temperature.md) is $T_F=E_F/k_B$.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C10](../../c10.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
