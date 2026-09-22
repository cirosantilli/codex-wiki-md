<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $r$ brackets the control-zero branch still does nothing, and the control-one branch applies $G^r$ to the target. Immediately before the final two [Hadamard gates](../../../../hadamard-gate.md), the [quantum state](../../../../quantum-state.md) is

$$
\frac{|0\rangle|+\rangle+|1\rangle G^r|+\rangle}{\sqrt2}.
$$

For the [constant function](../../../../constant-function.md) with $k=0$, the [phase oracle](../../../../phase-oracle.md) is $U_f=-I$, so $G=(-X)(-I)=X$. Since $|+\rangle$ is an [eigenstate](../../../../eigenstate.md) of the [Pauli X gate](../../../../pauli-x-gate.md) with [eigenvalue](../../../../eigenvalue.md) $+1$, $G^r|+\rangle=|+\rangle$ for every integer $r$. The final two [Hadamard gates](../../../../hadamard-gate.md) therefore give

$$
\boxed{|\Psi_{k=0}(r)\rangle=|00\rangle,\qquad \langle Z\otimes I\rangle=+1.}
$$

In particular, the first [qubit](../../../../qubit.md) always ends in $|0\rangle$.

For the [constant function](../../../../constant-function.md) with $k=2$, $U_f=I$ and $G=-X$, so $G^r|+\rangle=(-1)^r|+\rangle$. Thus the target remains in $|+\rangle$, and the top [qubit](../../../../qubit.md) before its final [Hadamard gate](../../../../hadamard-gate.md) is $(|0\rangle+(-1)^r|1\rangle)/\sqrt2$. The sign is a [relative quantum phase](../../../../relative-quantum-phase.md) between the control branches. The [Hadamard gate](../../../../hadamard-gate.md) converts it into the [integer parity](../../../../parity-mathematics.md) of $r$:

$$
\boxed{|\Psi_{k=2}(r)\rangle=|r\bmod2\rangle\otimes|0\rangle,\qquad
\langle Z\otimes I\rangle=(-1)^r.}
$$

The first [qubit](../../../../qubit.md) is therefore $|0\rangle$ for even $r$ and $|1\rangle$ for odd $r$, including all requested $r>1$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [5](../../5-split.md)
3. [2006](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
