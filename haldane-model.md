# Haldane model

↑ **Parent:** [Chern insulator](chern-insulator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Haldane_model)

[F. Duncan M. Haldane](f-duncan-m-haldane.md)'s 1988 [tight-binding model](tight-binding.md) adds complex second-neighbour hopping and opposite sublattice offsets to a [honeycomb lattice](honeycomb-lattice.md). Directed phases break [time-reversal symmetry](t-symmetry.md) while each primitive cell has zero net [magnetic flux](magnetic-flux.md). Smaller loops can enclose [magnetic flux](magnetic-flux.md); ordinary [Bloch states](bloch-state.md) remain available.[Haldane (1988), pp. 2015–2016, Fig. 1 and Eq. (1)](model-for-a-quantum-hall-effect-without-landau-levels-condensed-matter-realization-of-the-parity-anomaly-by-f-duncan-m-haldane.md)

Extend the [nearest-neighbour model of graphene](nearest-neighbour-model-of-graphene.md), ignoring physical [spin](spin.md) and interactions. With bond length $a$, $t_1>0$, $t_2\geq0$ and ordered sublattice basis $(A,B)$, choose

$$
\begin{aligned}
\boldsymbol\delta_1&=a(0,1),&
\boldsymbol\delta_2&=a(\sqrt3/2,-1/2),&
\boldsymbol\delta_3&=a(-\sqrt3/2,-1/2),\\
\mathbf b_1&=\boldsymbol\delta_3-\boldsymbol\delta_2,&
\mathbf b_2&=\boldsymbol\delta_1-\boldsymbol\delta_3,&
\mathbf b_3&=\boldsymbol\delta_2-\boldsymbol\delta_1,\\
f(\mathbf k)&=\sum_{j=1}^3e^{i\mathbf k\cdot\boldsymbol\delta_j}.&&&&
\end{aligned}
$$

The following [Bloch Hamiltonian](bloch-hamiltonian.md) defines $\phi$; reversing directed second-neighbour hopping sends $\phi\mapsto-\phi$:

$$
\begin{aligned}
d_0&=2t_2\cos\phi\sum_j\cos(\mathbf k\cdot\mathbf b_j),\\
d_x&=-t_1\operatorname{Re}f,&d_y&=t_1\operatorname{Im}f,\\
d_z&=M-2t_2\sin\phi\sum_j\sin(\mathbf k\cdot\mathbf b_j),\\
H&=\begin{pmatrix}d_0+d_z&-t_1f\\-t_1f^*&d_0-d_z\end{pmatrix},&
E_\pm&=d_0\pm\sqrt{t_1^2|f|^2+d_z^2}.
\end{aligned}
$$

The [Pauli matrices](pauli-matrices.md) act on sublattice amplitudes, as in [sublattice pseudospin in graphene](sublattice-pseudospin-in-graphene.md). The [identity matrix](identity-matrix.md) term $d_0I$ shifts both [energy eigenvalues](energy-eigenvalue-split.md) equally at each momentum; it changes neither the [eigenvectors](eigenvector.md) nor the direct separation $E_+-E_-$. A genuine [band insulator](band-insulator.md) additionally needs $\min_{\mathbf k}E_+>\max_{\mathbf k}E_-$. We use $t_2/t_1=0.08$ in the figures, within the original paper's sufficient nonoverlap restriction $|t_2/t_1|<1/3$.[Haldane (1988), p. 2016, immediately after Eq. (1): nonoverlapping bands](model-for-a-quantum-hall-effect-without-landau-levels-condensed-matter-realization-of-the-parity-anomaly-by-f-duncan-m-haldane.md)

**Table of contents**

- [Valley masses of the Haldane model](valley-masses-of-the-haldane-model.md)
- [Chern number of the Haldane model](chern-number-of-the-haldane-model.md)
- [Cold-atom realization of the Haldane model](cold-atom-realization-of-the-haldane-model.md)

## ↑ Ancestors (6)

1. [Chern insulator](chern-insulator.md)
2. [Topological quantum matter](topological-quantum-matter-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chern insulator](chern-insulator.md)
- [Cold-atom realization of the Haldane model](cold-atom-realization-of-the-haldane-model.md)
- [Valley masses of the Haldane model](valley-masses-of-the-haldane-model.md)
