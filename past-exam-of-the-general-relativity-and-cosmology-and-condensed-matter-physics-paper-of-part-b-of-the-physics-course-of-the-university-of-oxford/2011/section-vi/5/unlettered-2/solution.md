<h1 id="section-vi/5/unlettered-2/solution">Solution</h1>

↑ **Parent:** [Unlettered 2](../unlettered-2.md)

Write $\mathbf r=\sum_i s_i\mathbf a_i$. The [electron density](../../../../../electron-density.md) is periodic with period one in each $s_i$, so its three-dimensional [Fourier series](../../../../../fourier-series-split.md) has integer harmonics:

$$
\rho(\mathbf r)=\sum_{h,k,l\in\mathbb Z}\rho_{hkl}e^{2\pi i(hs_1+ks_2+ls_3)}
=\boxed{\sum_{\mathbf G}\rho_{\mathbf G}e^{i\mathbf G\cdot\mathbf r}.}
$$

If $\Omega$ is a [primitive unit cell](../../../../../primitive-unit-cell.md) of volume $\Omega_c$, [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives

$$
\rho_{\mathbf G}=\frac1{\Omega_c}\int_\Omega\rho(\mathbf r)e^{-i\mathbf G\cdot\mathbf r}\,d^3r.
$$

Conversely, translation by $\mathbf a_i$ multiplies a general [plane wave](../../../../../plane-wave.md) by $e^{i\mathbf q\cdot\mathbf a_i}$. Periodicity permits only $\mathbf q\cdot\mathbf a_i\in2\pi\mathbb Z$, precisely the [reciprocal lattice vectors](../../../../../reciprocal-lattice-vector.md). For a physical bounded periodic [electron density](../../../../../electron-density.md), the expansion exists in the usual square-integrable sense.

## ↑ Ancestors (13)

1. [Unlettered 2](../unlettered-2.md)
2. [5](../../5.md)
3. [Section VI](../../../section-vi.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the general relativity and cosmology and condensed matter physics paper of Part B of the physics course of the University of Oxford](../../../../split.md)
6. [General relativity and cosmology and condensed matter physics paper of Part B of the physics course of the University of Oxford](../../../../../general-relativity-and-cosmology-and-condensed-matter-physics-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
