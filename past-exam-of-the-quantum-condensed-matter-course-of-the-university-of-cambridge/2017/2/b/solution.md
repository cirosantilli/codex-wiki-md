<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A primitive cell containing two atoms has two independent displacement coordinates for each chosen polarization. Their coupled [normal modes](../../../../normal-mode.md) split into an [acoustic phonon branch](../../../../acoustic-phonon-branch.md), which translates the cell at long wavelength, and an [optical phonon branch](../../../../optical-phonon-branch.md), which moves its constituents against one another. The nonzero restoring force for the relative displacement gives a nonzero optical [frequency](../../../../frequency.md) even at the zone centre.

For an explicit scalar model, take alternating masses $M,m$, equal nearest-neighbor [spring constant](../../../../spring-constant.md) $K$, and cell length $a$. If $u_n,v_n$ are the displacements of the two atoms in cell $n$, [Newton's second law](../../../../newton-s-second-law.md) gives

$$
M\ddot u_n=K(v_n+v_{n-1}-2u_n),\qquad m\ddot v_n=K(u_n+u_{n+1}-2v_n).
$$

A mode proportional to $e^{i(kna-\omega t)}$ has a nonzero amplitude only when the two-by-two dynamical determinant vanishes. The resulting [diatomic-chain dispersion relation with equal springs](../../../../diatomic-chain-dispersion-relation-with-equal-springs.md), in this cell-length convention, is

$$
\boxed{\omega_\pm^2(k)=K\left(\frac1M+\frac1m\right)\pm K\sqrt{\left(\frac1M+\frac1m\right)^2-\frac4{Mm}\sin^2\frac{ka}{2}},\qquad |k|\leq\frac\pi a.}
$$

The minus branch is acoustic, with $\omega_-(0)=0$ and a linear small-$|k|$ dispersion. The plus branch is optical, with

$$
\boxed{\omega_+^2(0)=2K\left(\frac1M+\frac1m\right).}
$$

At $k=0$, the acoustic eigenvector has $u=v$. The optical eigenvector instead satisfies $Mu+mv=0$: its cell [centre of mass](../../../../center-of-mass.md) stays fixed while the atoms move oppositely. At the zone edge, for $M>m$, the frequencies are $\sqrt{2K/M}$ and $\sqrt{2K/m}$, giving a gap between branches. Both slopes vanish there. The dispersion and displacement patterns are shown in the preceding original figure.

If the two atoms carry opposite effective charges, the relative motion creates an oscillating [electric dipole moment](../../../../electric-dipole-moment.md), enabling [infrared](../../../../infrared.md) absorption by long-wavelength [light](../../../../light.md). The [photon](../../../../photon.md) [momentum](../../../../momentum-split.md) is tiny compared with the zone size, so ordinary optical absorption principally excites modes close to $k=0$. Raman activity instead depends on modulation of polarizability; the name optical does not imply that every such mode is [infrared](../../../../infrared.md) active. Three-dimensional crystals have separate longitudinal and transverse polarizations, and long-range Coulomb forces can split their optical frequencies. A monatomic primitive cell has no internal relative coordinate and therefore no optical branch of this type.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
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
