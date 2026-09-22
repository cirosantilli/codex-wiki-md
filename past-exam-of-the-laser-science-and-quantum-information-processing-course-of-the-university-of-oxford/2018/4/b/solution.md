<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $\sigma_\phi^2=I$, the [rotation gate](../../../../rotation-gate.md) is

$$
\boxed{R_\phi(\theta)=\begin{pmatrix}\cos(\theta/2)&-i e^{-i\phi}\sin(\theta/2)\\-i e^{i\phi}\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}.}
$$

For two chronological $\pi$ pulses, later operations multiply on the left:

$$
\boxed{R_{\phi_2}(\pi)R_{\phi_1}(\pi)=-\begin{pmatrix}e^{-i(\phi_2-\phi_1)}&0\\0&e^{i(\phi_2-\phi_1)}\end{pmatrix}=-R_z[2(\phi_2-\phi_1)].}
$$

Thus equatorial pulses generate arbitrary rotations about the $z$-axis. The minus sign is an overall [global phase](../../../../global-phase.md).

For the other chronological sequence, $T^4=Z$, and

$$
\boxed{H T^4=HZ=\frac1{\sqrt2}\begin{pmatrix}1&-1\\1&1\end{pmatrix}=R_y(\pi/2).}
$$

This equality has no additional overall [phase](../../../../phase-waves.md) under the standard definitions of $H$ and $T$. Rotations about two nonparallel axes, such as $x$ and $y$, generate all single-qubit operations by an [Euler angles](../../../../euler-angles.md) decomposition. Equivalently, the available equatorial rotations include $R_y(\pi/2)$ and arbitrary $R_z$ rotations constructed above; for example $H=R_y(\pi/2)Z$ and $T=e^{i\pi/8}R_z(\pi/4)$. Hence these rotations provide a universal single-qubit set. Overall [phases](../../../../phase-waves.md) do not affect any [probability](../../../../probability.md) or isolated-register observable; a [phase](../../../../phase-waves.md) controlled by an additional [qubit](../../../../qubit.md) would instead be relative and could not be discarded without accounting for it.

The minimum number of distinct fixed rotation gates for approximate universality is **two**. One fixed gate and its powers generate a commuting subgroup and cannot approximate all noncommuting single-qubit operations. Two suitable equatorial gates suffice: for example $R_x(\pi/\sqrt2)$ and $R_y(\pi/\sqrt3)$. Each has an angle irrational relative to $2\pi$, so its powers densely approximate rotations about its axis; combining the two supplies the Euler decomposition. Noncommutation alone is insufficient: two Clifford quarter-turns can generate only a finite subgroup. If continuous angles are regarded as available controls, two nonparallel rotation axes likewise suffice, now for exact Euler synthesis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
