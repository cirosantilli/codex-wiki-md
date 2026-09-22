<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Differentiating the specified rotating-frame amplitudes gives the time-independent [Schrödinger equation](../../../../schrodinger-equation.md)

$$
i\frac{d}{dt}\begin{pmatrix}\widetilde c_1\\\widetilde c_2\end{pmatrix}
=\frac12\begin{pmatrix}\delta&\Omega\\\Omega&-\delta\end{pmatrix}
\begin{pmatrix}\widetilde c_1\\\widetilde c_2\end{pmatrix}.
$$

The [characteristic polynomial](../../../../characteristic-polynomial.md) is $\lambda^2-(\delta^2+\Omega^2)/4=0$, hence

$$
\lambda_\pm=\pm\frac12\sqrt{\delta^2+\Omega^2}.
$$

For $\Omega\ne0$, corresponding normalized [eigenvectors](../../../../eigenvector.md) are proportional to $(\Omega,2\lambda_\pm-\delta)^T$. Their arbitrary complex coefficients evolve as $e^{-i\lambda_\pm t}$; this solves the amplitude equations for any initial [quantum state](../../../../quantum-state.md).

Restoring the common [energy](../../../../energy-split.md) origin $\overline E=(E_1+\hbar\omega+E_2)/2$, the two [dressed state](../../../../dressed-state.md) [energy eigenvalues](../../../../energy-eigenvalue-split.md) are

$$
E_\pm=\overline E\pm\frac\hbar2\sqrt{\delta^2+\Omega^2}.
$$

Thus their positive [energy](../../../../energy-split.md) separation increases by

$$
\boxed{\Delta(E_+-E_-)=\hbar[\sqrt{\delta^2+\Omega^2}-|\delta|]
=\frac{\hbar\Omega^2}{2|\delta|}+O(\Omega^4/|\delta|^3).}
$$

Equivalently, the branches connected to $E_1'=E_1+\hbar\omega$ and $E_2$ shift by $+\hbar\Omega^2/(4\delta)$ and $-\hbar\Omega^2/(4\delta)$ respectively. Their _signed_ difference $E_1'-E_2$ changes by $\hbar\Omega^2/(2\delta)$, which is the printed expression with a signed convention. For negative [Rabi detuning](../../../../rabi-detuning.md), an actual positive separation still increases; for example at $\delta=-10\Omega$ it cannot have the negative change implied by reading the printed expression as an unsigned gap. These opposite [AC Stark shifts](../../../../ac-stark-shift.md) describe level repulsion.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
