<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take a normalized environment [quantum state](../../../../../../quantum-state.md)

$$
\boxed{|\psi_E\rangle=\sqrt{1-\epsilon}|0\rangle+\sqrt\epsilon|1\rangle.}
$$

The [Controlled-Z gate](../../../../../../controlled-z-gate.md) is symmetric between the two [qubits](../../../../../../qubit.md), so it can be written with the environment as the controlling system:

$$
C_Z=I\otimes|0\rangle\langle0|+Z\otimes|1\rangle\langle1|.
$$

Expanding the joint [density operator](../../../../../../density-matrix.md) after the interaction gives

$$
\begin{aligned}
C_Z(\rho\otimes|\psi_E\rangle\langle\psi_E|)C_Z
={}&(1-\epsilon)\rho\otimes|0\rangle\langle0|+\epsilon Z\rho Z\otimes|1\rangle\langle1|\\
&+\sqrt{\epsilon(1-\epsilon)}\bigl(\rho Z\otimes|0\rangle\langle1|+Z\rho\otimes|1\rangle\langle0|\bigr).
\end{aligned}
$$

In the [partial trace](../../../../../../partial-trace.md), the two off-diagonal environment operators have trace zero, while each diagonal projector has trace one. Hence

$$
\boxed{\operatorname{tr}_E\!\left[C_Z(\rho\otimes|\psi_E\rangle\langle\psi_E|)C_Z\right]
=(1-\epsilon)\rho+\epsilon Z\rho Z=D_\epsilon(\rho).}
$$

Equivalently, the [Kraus operators](../../../../../../kraus-operator.md) are $K_0=\sqrt{1-\epsilon}I$ and $K_1=\sqrt\epsilon Z$, and $K_0^\dagger K_0+K_1^\dagger K_1=I$. This explicit [Stinespring dilation](../../../../../../stinespring-dilation.md) describes the system's dephasing by discarding information in the environment. A fresh environment in this state at each storage interval also realizes the memoryless iteration used in part (a).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
