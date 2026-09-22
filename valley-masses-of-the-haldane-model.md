# Valley masses of the Haldane model

↑ **Parent:** [Haldane model](haldane-model.md)

The only zeros of $f$, modulo the [reciprocal lattice](reciprocal-lattice.md), are the two [Dirac valleys in graphene](dirac-valleys-in-graphene.md),

$$
\mathbf K_\tau=\left(\tau\frac{4\pi}{3\sqrt3a},0\right),\qquad \tau=\pm1.
$$

At these momenta $\sum_j\sin(\mathbf K_\tau\cdot\mathbf b_j)=\tau3\sqrt3/2$. Thus the two [Dirac mass](dirac-mass-term.md) coefficients, measured in [energy](energy-split.md) units, are $m_\tau=M-\tau\mu$, with $\mu=3\sqrt3t_2\sin\phi$. For $\mathbf k=\mathbf K_\tau+\mathbf q$,

$$
H_\tau-d_0(\mathbf K_\tau)I=\hbar v(\tau q_x\sigma_x+q_y\sigma_y)+m_\tau\sigma_z+O(|\mathbf q|^2),
\qquad v=\frac{3t_1a}{2\hbar}.
$$

The two [Dirac cones](dirac-cone.md) have opposite orientation, encoded by $\tau$. A scalar sublattice offset $M$ gives equal-sign [Dirac masses](dirac-mass-term.md); imaginary second-neighbour hopping at $M=0$ gives opposite-sign [Dirac masses](dirac-mass-term.md). Both mechanisms open valley gaps

$$
\Delta_\tau=E_+(\mathbf K_\tau)-E_-(\mathbf K_\tau)=2|m_\tau|.
$$

An observed [band gap](band-gap.md) alone therefore cannot establish a [Chern insulator](chern-insulator.md). In particular, the gapless [nearest-neighbour model of graphene](nearest-neighbour-model-of-graphene.md) and its sublattice-mass deformation should not be confused with the topologically nontrivial [Haldane model](haldane-model.md).

A [band gap](band-gap.md) closes when all three components of $\mathbf d$ vanish. Since $d_x=d_y=0$ only at the two valleys, the phase boundaries are exactly $M=\pm3\sqrt3t_2\sin\phi$. Usually one valley becomes massless; at $M=0$, $\sin\phi=0$, both do. The occupied-band [Chern number](chern-number.md) is undefined at every such touching, even if a numerical momentum grid misses its location.

<a id="image-haldane-phases-meet-where-a-valley-gap-closes"></a>
![](haldane-chern-phase-and-valley-gaps.png)

**[Figure 3](#image-haldane-phases-meet-where-a-valley-gap-closes). Haldane phases meet where a valley gap closes**. [Source](haldane-chern-phase-and-valley-gaps.py). Original model calculation with the stated lower-band Berry-connection convention and $t_2/t_1=0.08$. Left: integer Chern numbers; black curves denote singular parameters, where no Chern number is assigned. Right: the two valley gaps along $\phi=\pi/2$; the vertical axis shows valley gaps, rather than an assumption about global band extrema. No experimental data are plotted.

## ↑ Ancestors (7)

1. [Haldane model](haldane-model.md)
2. [Chern insulator](chern-insulator.md)
3. [Topological quantum matter](topological-quantum-matter-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
