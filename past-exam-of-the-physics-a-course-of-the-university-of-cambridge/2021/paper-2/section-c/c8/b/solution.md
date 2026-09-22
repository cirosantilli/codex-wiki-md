<h1 id="section-c/c8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [Fourier series](../../../../../../fourier-series-split.md) convention

$$
V(x)=\sum_{j\in\mathbb Z}V_j e^{ijG_1x},\qquad
V_j=\frac1a\int_0^aV(x)e^{-ijG_1x}\,dx.
$$

For a real [potential energy](../../../../../../potential-energy.md), $V_{-1}=V_1^*$. The symbol $V(G_1)$ means the [Fourier coefficient](../../../../../../fourier-coefficient.md) $V_1$, with units of [energy](../../../../../../energy-split.md), rather than the pointwise value of $V(x)$ at a position $G_1$.

Retain the two [plane waves](../../../../../../plane-wave.md) $|1\rangle=L^{-1/2}e^{ikx}$ and $|2\rangle=L^{-1/2}e^{i(k-G_1)x}$ in the [nearly-free electron model](../../../../../../nearly-free-electron-model.md). Their kinetic [energies](../../../../../../energy-split.md) are $\epsilon_1=\hbar^2k^2/(2m)$ and $\epsilon_2=\hbar^2(k-G_1)^2/(2m)$. The [matrix representation of a linear map](../../../../../../matrix-representation-of-a-linear-map.md) for the [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) projected onto this two-dimensional [basis](../../../../../../basis.md) is

$$
H=\begin{pmatrix}\epsilon_1+V_0&V_1\\V_1^*&\epsilon_2+V_0\end{pmatrix}.
$$

Thus $\det(H-EI)=0$ gives

$$
(E-V_0-\epsilon_1)(E-V_0-\epsilon_2)-|V_1|^2=0.
$$

Solving this [quadratic equation](../../../../../../quadratic-equation.md) yields

$$
\boxed{E_\pm=V_0+\frac{\epsilon_1+\epsilon_2}{2}
\pm\frac12\sqrt{(\epsilon_1-\epsilon_2)^2+4|V_1|^2}.}
$$

Choosing the zero of [potential energy](../../../../../../potential-energy.md) so that its spatial average is $V_0=0$ reproduces the requested expression. If that average has not been removed, both [energy bands](../../../../../../energy-band.md) are shifted by $V_0$; no [band gap](../../../../../../band-gap.md), [group velocity](../../../../../../group-velocity.md) or [effective mass](../../../../../../band-effective-mass.md) is changed by this constant shift.

The two kinetic [energies](../../../../../../energy-split.md) coincide at $k=G_1/2$. Their coupling gives an [avoided crossing](../../../../../../avoided-crossing.md) with [band gap](../../../../../../band-gap.md) $2|V_1|$. The result is exact within the projected two-wave [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md). It is an approximation to the full crystal problem, appropriate near this crossing for a weak [periodic potential](../../../../../../periodic-potential.md) whose other [Fourier coefficients](../../../../../../fourier-coefficient.md) do not cause strong mixing with remote [plane waves](../../../../../../plane-wave.md). Small $|V_1|$ alone would not justify ignoring arbitrarily large other [Fourier coefficients](../../../../../../fourier-coefficient.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
