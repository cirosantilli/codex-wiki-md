<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\bar\chi=(\chi_1+\chi_2)/2$ and $\delta\chi=\chi_2-\chi_1$. Since the supplied [rotation matrix](../../../../rotation-matrix.md) is real and orthogonal, $U^{-1}=U^T$. Direct [matrix multiplication](../../../../matrix-multiplication.md) gives the flavor-basis [Hamiltonian](../../../../hamiltonian.md)

$$
H'=\begin{pmatrix}\chi_1c^2+\chi_2s^2&(\chi_2-\chi_1)sc\\(\chi_2-\chi_1)sc&\chi_1s^2+\chi_2c^2\end{pmatrix}
=\boxed{\bar\chi I+\frac{\delta\chi}{2}\begin{pmatrix}-\cos2\theta&\sin2\theta\\\sin2\theta&\cos2\theta\end{pmatrix}.}
$$

The common term $\bar\chi I$ produces only an overall quantum phase. The off-diagonal elements $H'_{e\mu}=H'_{\mu e}=(\delta\chi/2)\sin2\theta$ couple the two [interaction eigenstates](../../../../interaction-eigenstate.md) in the [Schrödinger equation](../../../../schrodinger-equation.md). Flavor change requires both $\delta\chi\ne0$ and $\sin2\theta\ne0$. For [ultrarelativistic neutrinos](../../../../ultrarelativistic-neutrino.md) in vacuum, $\delta\chi\simeq\Delta m^2/(2E)$, so a nonzero squared-[mass](../../../../mass.md) difference is needed. Observable [neutrino oscillation](../../../../neutrino-oscillation.md) also requires coherent production and propagation of the two components and a resolvable nonzero relative phase; special propagation times can return the initial flavor even when these Hamiltonian conditions hold.

A useful distinction for the next part is that $H'_{ee}$ is an [energy](../../../../energy-split.md), not a time-dependent survival [probability amplitude](../../../../probability-amplitude.md). The latter is the $ee$ element of $S(t)=\exp(-iH't)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
