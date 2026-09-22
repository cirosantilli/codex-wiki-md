<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an [orthonormal basis](../../../../orthonormal-basis.md) of [stationary states](../../../../stationary-state.md) and project the [Time-dependent Schrödinger equation](../../../../time-dependent-schrodinger-equation.md) onto state 2 after removing its free-evolution phase. The stationary [Hamiltonian](../../../../hamiltonian.md) terms cancel the derivatives of those phases, leaving

$$
i\hbar\dot c_2=V_{21}(t)e^{i(E_2-E_1)t/\hbar}c_1+V_{22}(t)c_2.
$$

Define $d_{21}=\langle\psi_2|ex|\psi_1\rangle$ and $d_{22}=\langle\psi_2|ex|\psi_2\rangle$. With the supplied [time-dependent quantum perturbation](../../../../time-dependent-quantum-perturbation.md),

$$
\boxed{\omega_0=\frac{E_2-E_1}{\hbar},\qquad
\Omega=\frac{\mathcal E d_{21}}{\hbar},\qquad
V_{22}(t)=\mathcal E d_{22}\cos\omega t,}
$$

and therefore $\dot c_2=-i\Omega\cos(\omega t)e^{i\omega_0t}c_1-iV_{22}c_2/\hbar$. The state phases may be chosen so $d_{21}$ and $\Omega$ are real for this single driven pair; otherwise [probabilities](../../../../probability.md) depend on $|\Omega|^2$ and the conjugate [matrix element](../../../../matrix-element.md) appears in the equation for $c_1$. Our $\Omega$ is the resonant [Rabi angular frequency](../../../../rabi-angular-frequency.md) in the usual convention whose rotating-wave off-diagonal [Hamiltonian](../../../../hamiltonian.md) is $\hbar\Omega/2$.

For a field-free atom with symmetry under [spatial reflection](../../../../spatial-reflection.md), each selected nondegenerate stationary orbital can be chosen with definite [parity](../../../../parity.md). Since $x$ is odd, $\langle2|x|2\rangle=-\langle2|x|2\rangle$, so $V_{22}=0$; the same reasoning gives $V_{11}=0$. **Being an [energy eigenstate](../../../../energy-eigenstate.md) alone is not sufficient.** As an explicit mathematical counterexample, a displaced [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md) with potential proportional to $(x-x_c)^2$ has [energy eigenstates](../../../../energy-eigenstate.md) with $\langle x\rangle=x_c$, giving $V_{22}=e\mathcal E x_c\cos\omega t$ when $x_c\ne0$. The vanishing used in the atomic model rests on its [parity](../../../../parity.md) assumption, not merely on stationarity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum, atomic and molecular physics course of the University of Oxford](../../../split.md)
5. [Quantum, atomic and molecular physics course of the University of Oxford](../../../../quantum-atomic-and-molecular-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
