<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [geometric quantum state synthesis by adjacent rotations](../../../../../../geometric-quantum-state-synthesis-by-adjacent-rotations.md), rather than three full [level population](../../../../../../quantum-state-population.md) swaps. Each resonant pulse implements a complex [Givens rotation](../../../../../../givens-rotation.md) on one allowed two-state plane. Start with the target amplitude vector, use such rotations to eliminate entries back to the first basis vector, and reverse that sequence. Its angles are fixed by the ratios of target amplitudes, and optical phases supply their relative complex phases.

Here is an explicit real-coordinate construction in the interaction picture. Define a phase-calibrated rotation by

$$
R_{jk}(\beta)|j\rangle=\cos\beta|j\rangle+\sin\beta|k\rangle,\qquad
R_{jk}(\beta)|k\rangle=-\sin\beta|j\rangle+\cos\beta|k\rangle.
$$

A resonant [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) proportional to $-i|j\rangle\langle k|+i|k\rangle\langle j|$ realizes this rotation; the optical phase chooses that quadrature. Let $\beta=\arccos(1/\sqrt3)$. Then

$$
\begin{aligned}
|1\rangle&\xrightarrow{R_{12}(\beta)}\frac{|1\rangle+\sqrt2|2\rangle}{\sqrt3}\\
&\xrightarrow{R_{23}(3\pi/4)}\frac{|1\rangle-|2\rangle+|3\rangle}{\sqrt3}\\
&\xrightarrow{R_{34}(\pi/2)}\boxed{\frac{|1\rangle-|2\rangle+|4\rangle}{\sqrt3}}.
\end{aligned}
$$

The pulse areas equal these rotation parameters in the direct Hamiltonian-coefficient convention of [quantum pulse area](../../../../../../quantum-pulse-area.md). A given sign or phase choice for a physical transition depends on its dipole and basis conventions; calibration realizes the specified rotation without assuming every adjacent transition has the same energy ordering.

If the requested amplitudes refer to the laboratory frame at $t_F$, the target for this construction is $U_0(t_F,0)^\dagger|\Psi\rangle$, not simply $|\Psi\rangle$. Set the rotation phases accordingly, or add the equivalent accessible diagonal phase corrections. This compensates the known drift phases and gives the stated laboratory superposition, not merely the correct [level populations](../../../../../../quantum-state-population.md). Strong regularity and connected allowed transitions guarantee the required controllability; bandwidth restrictions set how slowly the selective approximation must be implemented.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
