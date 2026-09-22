# Quadratic short-time quantum survival probability

↑ **Parent:** [Unitary time evolution](unitary-time-evolution.md)

For a normalized [quantum state](quantum-state.md) $\psi$ and a [self-adjoint operator](self-adjoint-operator.md) $H$ on a finite-dimensional [Hilbert space](hilbert-space-split.md), expand its [unitary time evolution](unitary-time-evolution.md):

$$
\langle\psi,e^{-iHt/\hbar}\psi\rangle
=1-\frac{i\langle H\rangle t}{\hbar}-\frac{\langle H^2\rangle t^2}{2\hbar^2}+O(t^3).
$$

Multiplying by its [complex conjugate](complex-conjugate.md) gives the survival [probability](probability.md)

$$
|\langle\psi,e^{-iHt/\hbar}\psi\rangle|^2
=1-\frac{\langle H^2\rangle-\langle H\rangle^2}{\hbar^2}t^2+O(t^4).
$$

The function is even in $t$, so its odd coefficients vanish. The coefficient $(\Delta H)^2=\langle H^2\rangle-\langle H\rangle^2$ is the [variance](variance-split.md) of the [energy](energy-split.md). This quadratic departure yields the [quantum Zeno effect](quantum-zeno-effect.md) when ideal [projective measurements](projective-measurement.md) repeatedly reset the [quantum state](quantum-state.md).

## ↑ Ancestors (9)

1. [Unitary time evolution](unitary-time-evolution.md)
2. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
3. [Observable](observable.md)
4. [Quantum state](quantum-state.md)
5. [Quantum system](quantum-system-split.md)
6. [Quantum mechanics](quantum-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/5/3/solution.md)
- [Solution](past-exam-of-the-quantum-theory-course-of-the-university-of-oxford/2021/3/b/iii/solution.md)
- [Quantum Zeno effect](quantum-zeno-effect.md)
