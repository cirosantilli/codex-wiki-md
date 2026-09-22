<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the ordered [orthonormal basis](../../../../orthonormal-basis.md) $(|1s\rangle,|2p_x\rangle)$. The projected [Hamiltonian](../../../../hamiltonian.md) between pulses is $H_0=-\Delta\sigma_z$, so its free [time-evolution operator](../../../../time-evolution-operator.md) through a period is

$$
U_\Delta=e^{i\alpha\sigma_z}=\begin{pmatrix}e^{i\alpha}&0\\0&e^{-i\alpha}\end{pmatrix},\qquad \alpha=\frac{\Delta\tau}{\hbar}.
$$

Across one instantaneous pulse, integrating the [Schrödinger equation](../../../../schrodinger-equation.md) gives

$$
U_E=e^{-i\beta\sigma_x}=\begin{pmatrix}\cos\beta&-i\sin\beta\\-i\sin\beta&\cos\beta\end{pmatrix},\qquad \beta=\frac{Ex_0\tau}{\hbar},
$$

using the [exponential of a Pauli vector](../../../../exponential-of-a-pauli-vector.md). The finite free [Hamiltonian](../../../../hamiltonian.md) contributes vanishing evolution during the zero-duration kick. A period measured immediately before successive pulses therefore consists of the kick followed by free evolution. Composition gives

$$
\boxed{U(N\tau-\epsilon,-\epsilon)=(U_\Delta U_E)^N,\qquad\epsilon\to0^+.}
$$

This is the [Floquet operator](../../../../floquet-operator.md) at the specified phase of the pulse train. Actual hydrogenic [energy levels](../../../../energy-level.md) are not opposite numbers: the displayed convention subtracts their midpoint, with $\Delta=(E_{2p}-E_{1s})/2$. Restoring that midpoint multiplies the result by an unobservable [global phase](../../../../global-phase.md). Likewise $E$ in the given [Hamiltonian](../../../../hamiltonian.md) denotes the electric coupling per unit length; if it is instead a physical electric-field strength, its charge factor must be included in $Ex_0$.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
