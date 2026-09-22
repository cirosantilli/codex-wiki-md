<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $|0\rangle$ to have $\sigma_z=+1$ and use angular-frequency [gyromagnetic ratios](../../../../gyromagnetic-ratio.md). Neglecting interspin coupling, the [Hamiltonian](../../../../hamiltonian.md) of the [Zeeman energy](../../../../zeeman-energy.md) is

$$
\boxed{H=-\frac{\hbar B}{2}(\gamma_1 Z_1+\gamma_2 Z_2).}
$$

For $\gamma_1=\gamma_2=\gamma$, define $\epsilon=\hbar\gamma B/(k_BT)$. The exact thermal [density matrix](../../../../density-matrix-split.md) in the order $|00\rangle,|01\rangle,|10\rangle,|11\rangle$ is

$$
\rho_{\mathrm{th}}=\frac{\operatorname{diag}(e^\epsilon,1,1,e^{-\epsilon})}{4\cosh^2(\epsilon/2)}.
$$

At high [temperature](../../../../temperature-split.md), $|\epsilon|\ll1$, expand both numerator and normalization to obtain

$$
\boxed{\rho_{\mathrm{th}}=\frac14\operatorname{diag}(1+\epsilon,1,1,1-\epsilon)+O(\epsilon^2),\qquad \epsilon=\frac{\hbar\gamma B}{k_BT}.}
$$

For positive $\gamma$, $|00\rangle$ is the most populated state; a negative [gyromagnetic ratio](../../../../gyromagnetic-ratio.md) reverses that population preference under this basis convention.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
