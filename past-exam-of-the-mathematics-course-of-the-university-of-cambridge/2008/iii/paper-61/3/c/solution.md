<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a concrete variational method, maximize the terminal-observable objective with a fluence penalty,

$$
J[f]=\langle\psi(T)|A|\psi(T)\rangle-\frac\lambda2\int_0^Tf(t)^2dt,\qquad
 i\hbar\dot\psi=(H_0+fH_1)\psi,\quad\psi(0)=\psi_0,
$$

where $\lambda>0$ weights the control cost. Enforce the dynamics with a complex [costate](../../../../../../costate.md) $|\chi(t)\rangle$ and the real augmented functional

$$
\mathcal J=J-2\operatorname{Re}\int_0^T\left\langle\chi\left|\dot\psi+\frac i\hbar(H_0+fH_1)\psi\right.\right\rangle dt.
$$

Variation of $\chi$ restores the state equation. Integrate the $\dot\psi$ variation by parts; because $\delta\psi(0)=0$, the terminal coefficient gives $\chi(T)=A\psi(T)$, and the interior coefficient gives

$$
i\hbar\dot\chi=(H_0+fH_1)\chi.
$$

This equation has final data, so it is integrated backward. Variation of the real control gives the [variational costate gradient for Hamiltonian quantum control](../../../../../../variational-costate-gradient-for-hamiltonian-quantum-control.md)

$$
\boxed{\frac{\delta J}{\delta f(t)}=\frac2\hbar\operatorname{Im}\langle\chi(t)|H_1|\psi(t)\rangle-\lambda f(t).}
$$

In particular an unconstrained stationary pulse satisfies $f(t)=2\operatorname{Im}\langle\chi|H_1|\psi\rangle/(\lambda\hbar)$. The state, adjoint and control equations form a coupled two-boundary-value problem, so the stationarity formula is not an independent explicit solution for $f$.

Use [direct-adjoint looping](../../../../../../direct-adjoint-looping.md): start from an admissible pulse, propagate the state forward, set the terminal [costate](../../../../../../costate.md), propagate it backward, compute the [gradient](../../../../../../gradient.md) on the time grid, and update the pulse with an ascent step and line search. Project amplitude bounds and impose bandwidth constraints within the parametrization or update. Repeat until the projected [gradient](../../../../../../gradient.md) is small. For gate objectives the forward variable is the propagator and the [costate](../../../../../../costate.md) is matrix-valued; for mixed-state objectives it is the [density operator](../../../../../../density-matrix.md). [Gradient ascent pulse engineering](../../../../../../gradient-ascent-pulse-engineering.md) applies the same efficient forward/backward differentiation to time-slice amplitudes. The variational conditions identify local stationary controls and require numerical convergence checks; they do not prove global optimality of a nonconvex control landscape.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
