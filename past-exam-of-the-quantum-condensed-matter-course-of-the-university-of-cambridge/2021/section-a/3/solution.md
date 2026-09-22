<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let adjacent equal masses $m$ be separated by $a$, with alternating strong and weak spring constants $K$ and $\kappa$, $K\gg\kappa>0$. The pattern repeats after $2a$, even though the masses are identical. Thus the first [Brillouin zone](../../../../brillouin-zone.md) is

$$
\boxed{-\frac{\pi}{2a}\leq q\leq\frac{\pi}{2a}.}
$$

Choose the strong bond inside each two-atom [primitive unit cell](../../../../primitive-unit-cell.md). With displacement amplitudes $(u,v)e^{i(2naq-\omega t)}$, the [normal mode](../../../../normal-mode.md) equations are

$$
m\omega^2\begin{pmatrix}u\\v\end{pmatrix}
=\begin{pmatrix}K+\kappa&-K-\kappa e^{-2iqa}\\-K-\kappa e^{2iqa}&K+\kappa\end{pmatrix}
\begin{pmatrix}u\\v\end{pmatrix}.
$$

The [alternating-spring chain dispersion relation](../../../../alternating-spring-chain-dispersion-relation.md) is consequently

$$
\boxed{\omega_\pm^2(q)=\frac{K+\kappa\pm\sqrt{(K-\kappa)^2+4K\kappa\cos^2(qa)}}m.}
$$

The lower [acoustic phonon branch](../../../../acoustic-phonon-branch.md) has in-phase motion within the strongly bound pair and $\omega_-(0)=0$. Its small-$q$ slope is the [speed of sound](../../../../speed-of-sound.md),

$$
c_s=a\sqrt{\frac{2K\kappa}{m(K+\kappa)}}\simeq a\sqrt{\frac{2\kappa}{m}}.
$$

The upper [optical phonon branch](../../../../optical-phonon-branch.md) has opposite motion within each pair, with $\omega_+(0)=\sqrt{2(K+\kappa)/m}$. Here “optical” names the gapped branch; equal neutral masses need not couple to light through an electric dipole.

In the [strong-bond limit of the alternating-spring chain](../../../../strong-bond-limit-of-the-alternating-spring-chain.md), the pairs act almost as rigid dimers in the low-frequency branch, while their internal stretch gives a high, nearly flat branch:

$$
\omega_-^2\simeq\frac{2\kappa}{m}\sin^2(qa),\qquad
\omega_+^2\simeq\frac{2K}{m}+\frac{2\kappa}{m}\cos^2(qa).
$$

At the zone edge the two frequencies are $\sqrt{2\kappa/m}$ and $\sqrt{2K/m}$, separated by a large forbidden frequency interval. Neighbouring cells are out of phase there. Both branches have horizontal tangents at the edge.

<a id="section-a/3/image-phonon-branches-and-displacement-patterns-of-a-strongly-dimerized-equal-mass-chain"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021-q3-alternating-springs.png)

**[Figure 1](#section-a/3/image-phonon-branches-and-displacement-patterns-of-a-strongly-dimerized-equal-mass-chain). Phonon branches and displacement patterns of a strongly dimerized equal-mass chain**. Original calculation for $\kappa/K=0.06$. The horizontal coordinate uses the two-atom-cell Brillouin-zone boundary. Strong solid bonds and weak dashed bonds identify each dimer. Arrows show relative displacements at the zone centre and edge; their overall sign and amplitude are arbitrary.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
