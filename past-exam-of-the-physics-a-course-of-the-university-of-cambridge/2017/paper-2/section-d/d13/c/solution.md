<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [Bravais lattice](../../../../../../bravais-lattice.md) with primitive translation vectors $\mathbf a_1,\mathbf a_2,\mathbf a_3$, define the [reciprocal lattice](../../../../../../reciprocal-lattice.md) by vectors $\mathbf G$ satisfying $e^{i\mathbf G\cdot\mathbf R}=1$ for every direct-lattice translation $\mathbf R$. A convenient basis is

$$
\boxed{\mathbf b_1=2\pi\frac{\mathbf a_2\times\mathbf a_3}{\mathbf a_1\cdot(\mathbf a_2\times\mathbf a_3)}}
$$

with cyclic formulas for $\mathbf b_2,\mathbf b_3$. Then $\mathbf a_i\cdot\mathbf b_j=2\pi\delta_{ij}$ and $\mathbf G=h\mathbf b_1+k\mathbf b_2+l\mathbf b_3$ for integers $h,k,l$. The reciprocal primitive volume is $(2\pi)^3/V_{\rm cell}$.

These vectors are the spatial [Fourier series](../../../../../../fourier-series-split.md) frequencies of a periodic lattice potential or density. Elastic coherent crystal [diffraction](../../../../../../diffraction.md) occurs when the scattering [wavevector](../../../../../../wavevector.md) transfer equals a [reciprocal lattice](../../../../../../reciprocal-lattice.md) vector, with intensities additionally controlled by the basis [crystal lattice structure factor](../../../../../../crystal-lattice-structure-factor.md). This is the reciprocal-space version of [Bragg's law](../../../../../../bragg-s-law.md). A lattice of points and its basis should not be confused: a basis can make allowed reciprocal-lattice [diffraction](../../../../../../diffraction.md) intensities vanish.

The first [Brillouin zone](../../../../../../brillouin-zone.md) is the [Wigner-Seitz cell](../../../../../../wigner-seitz-cell.md) around the reciprocal origin: it consists of points closer to $\mathbf G=0$ than to any other reciprocal point. Its faces lie on the perpendicular bisectors

$$
\boxed{\mathbf k\cdot\mathbf G=|\mathbf G|^2/2}.
$$

To see the condition, equate $|\mathbf k|^2$ and $|\mathbf k-\mathbf G|^2$. These are also free-electron Bragg-degeneracy planes, where a periodic potential can open a [band gap](../../../../../../band-gap.md). Higher zones classify regions beyond successive Bragg planes; the reduced-zone description folds them into the first zone while retaining a band label.

In one dimension with spacing $a$, reciprocal points occur at $2\pi j/a$, and the first zone is $[-\pi/a,\pi/a]$. A square lattice of spacing $a$ has reciprocal basis $2\pi\hat{\mathbf x}/a,2\pi\hat{\mathbf y}/a$, and a square first zone with edges at $k_x,k_y=\pm\pi/a$.

<a id="section-d/d13/c/image-reciprocal-points-and-the-first-brillouin-zone-of-a-two-dimensional-square-lattice"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2-d13-reciprocal-zone.png)

**[Figure 8](#section-d/d13/c/image-reciprocal-points-and-the-first-brillouin-zone-of-a-two-dimensional-square-lattice). Reciprocal points and the first Brillouin zone of a two-dimensional square lattice**.

The reciprocal of a [face-centered cubic lattice](../../../../../../face-centered-cubic-lattice.md) is a [body-centered cubic lattice](../../../../../../body-centered-cubic-lattice.md) and vice versa, with the scale fixed by the primitive-vector definition. In a [Bloch state](../../../../../../bloch-state.md), [wavevectors](../../../../../../wavevector.md) differing by $\mathbf G$ describe equivalent crystal momenta modulo the lattice periodicity. A crystal with $N$ primitive cells has $N$ allowed [wavevectors](../../../../../../wavevector.md) in one Brillouin zone, hence $N$ states in each band per spin. This state count links reciprocal geometry to [band filling](../../../../../../band-filling.md), metallic conduction and band insulating behaviour. Reciprocal space also labels [phonons](../../../../../../phonon.md) and makes conservation of [crystal momentum](../../../../../../crystal-momentum.md) modulo $\hbar\mathbf G$ transparent.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
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
