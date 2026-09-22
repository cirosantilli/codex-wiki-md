<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A full fringe scan is unnecessary. Use the same components to make three fixed [projective measurements](../../../../../../projective-measurement.md), on separate batches of identically prepared [photons](../../../../../../photon.md). Direct path detection after the [polarizing beam splitter](../../../../../../polarizing-beam-splitter.md) measures the $H/V$ populations. Recombine after matching the arm [photon polarizations](../../../../../../photon-polarization.md), once with $\theta=0$ and once with $\theta=\pi/2$, to measure the two quadratures of the [quantum coherence](../../../../../../quantum-coherence-in-a-specified-basis.md).

In the $H/V$ basis, write the [density matrix](../../../../../../density-matrix.md) in terms of its [Bloch vector](../../../../../../bloch-vector.md) as $\rho=(I+r_xX+r_yY+r_zZ)/2$. The previous formula becomes

$$
P_1(\theta)=\frac12+\frac12(r_x\cos\theta-r_y\sin\theta).
$$

Thus three measured relative frequencies give

$$
\boxed{r_z=P(H)-P(V),\qquad r_x=2P_1(0)-1,\qquad r_y=1-2P_1(\pi/2),}
$$

and determine

$$
\boxed{\rho=\frac12\begin{pmatrix}1+r_z&r_x-ir_y\\r_x+ir_y&1-r_z\end{pmatrix}.}
$$

The two interferometric settings analyze the diagonal [linear polarizations](../../../../../../linear-polarization.md) $(|H\rangle\pm|V\rangle)/\sqrt2$ and the [circular polarizations](../../../../../../circular-polarization.md) $(|H\rangle\pm i|V\rangle)/\sqrt2$, with detector labels fixed by the calibrated [quantum phase](../../../../../../quantum-phase.md) convention. This is [informationally complete three-observable qubit tomography](../../../../../../informationally-complete-three-observable-qubit-tomography.md): direct measurements in three bases replace fitting an entire phase-dependent fringe. It also reconstructs a mixed input, for which $|r|\le1$, although the source here is assumed pure.

Simply measuring transmission through one fixed [polarizing beam splitter](../../../../../../polarizing-beam-splitter.md) would determine only $r_z$. Rotating a linear analyzer through different angles can additionally determine $r_x$, but cannot distinguish the two signs of $r_y$ without a relative-phase measurement. For arbitrary, possibly elliptical [photon polarization](../../../../../../photon-polarization.md), all three settings above are needed; no extra analyzer element beyond the described path-phase control and [photon polarization](../../../../../../photon-polarization.md) rotator is required.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
