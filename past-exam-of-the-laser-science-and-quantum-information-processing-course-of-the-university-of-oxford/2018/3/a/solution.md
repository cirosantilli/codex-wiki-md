<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $\sigma_z|e\rangle=|e\rangle$ and $\sigma_z|g\rangle=-|g\rangle$. In the resonant [Jaynes-Cummings model](../../../../jaynes-cummings-model.md), the interaction connects only $|e,n\rangle$ and $|g,n+1\rangle$. Both have free [energy](../../../../energy-split.md) $\hbar\omega(n+1/2)$, and their interaction [matrix](../../../../matrix.md) is $\hbar g\sqrt{n+1}\,\sigma_x$. Therefore

$$
H_n=\hbar\omega(n+1/2)I+\hbar g\sqrt{n+1}\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Exponentiating this two-state block and applying it to $|e,n\rangle$ yields

$$
\boxed{|\psi_n(t)\rangle=e^{-i\omega(n+1/2)t}\left[\cos(g\sqrt{n+1}\,t)|e,n\rangle-i\sin(g\sqrt{n+1}\,t)|g,n+1\rangle\right].}
$$

The populations undergo [Rabi oscillations](../../../../rabi-cycle.md) at [angular frequency](../../../../angular-frequency.md) $2g\sqrt{n+1}$. The common [phase](../../../../phase-waves.md) in this fixed-$n$ block does not affect its [probabilities](../../../../probability.md), but it must be retained when blocks with different [photon numbers](../../../../photon-number.md) are superposed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
