<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $U(t)=e^{-iHt/\hbar}$ and write $\psi_S(t)=U(t)\psi_0$ in the [Schrödinger picture](../../../../schrodinger-picture.md), with [observables](../../../../observable.md) $A_S$ constant unless they have an explicit time dependence. In the [Heisenberg picture](../../../../heisenberg-picture.md) the state is $\psi_H=\psi_0$ and

$$
A_H(t)=U(t)^*A_SU(t),\qquad\boxed{\dot A_H=\frac{i}{\hbar}[H,A_H]+U^*(\partial_tA_S)U.}
$$

Differentiate the two [unitary](../../../../unitary-connection.md) factors to obtain the equation. [Unitarity](../../../../unitary-operator.md) gives $\langle\psi_S,A_S\psi_S\rangle=\langle\psi_0,A_H\psi_0\rangle$.

For the [interaction picture](../../../../interaction-picture.md) choose a reference split $H=H_0+V$, put $U_0=e^{-iH_0t/\hbar}$, and define $\psi_I=U_0^*\psi_S$, $A_I=U_0^*A_SU_0$. Then $i\hbar\dot\psi_I=V_I\psi_I$, $V_I=U_0^*VU_0$, while $A_I$ evolves with $H_0$ (and its explicit time dependence). Again

$$
\boxed{\langle\psi_I,A_I\psi_I\rangle=\langle\psi_S,A_S\psi_S\rangle=\langle\psi_0,A_H\psi_0\rangle.}
$$

These are different [unitary](../../../../unitary-connection.md) allocations of the same dynamics between states and [observables](../../../../observable.md), so measured [expectations](../../../../expected-value-split.md) agree.

The [canonical commutation relation](../../../../canonical-commutation-relation.md) now gives

$$
\boxed{\dot X_t=P_t/m,\quad\dot P_t=-m\omega^2X_t-\mathcal E,\quad\dot A_t=-i\omega A_t-\mathcal E.}
$$

Multiplication of the last equation by $e^{i\omega t}$ and integration gives

$$
\boxed{A_t=e^{-i\omega t}A_0-\frac{i\mathcal E}{\omega}(e^{-i\omega t}-1).}
$$

Since $A_t^*-A_t=2im\omega X_t$ and $A_0\psi_0=0$, both initial [expectations](../../../../expected-value-split.md) of $A_0,A_0^*$ vanish. Therefore

$$
\boxed{\langle X_t\rangle=-\frac{\mathcal E}{m\omega^2}(1-\cos\omega t).}
$$

**The printed positive displacement endpoint has the wrong sign** for the [Hamiltonian](../../../../hamiltonian.md)'s positive $\mathcal EX$ term. The two turning values are $0$ and $-2\mathcal E/(m\omega^2)$; their ordering depends on the sign of $\mathcal E$. The result oscillates about the displaced equilibrium $-\mathcal E/(m\omega^2)$, exactly as the force $-\mathcal E$ predicts.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
