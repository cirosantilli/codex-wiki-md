<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A constant function has $f(0)=f(1)$, whereas a balanced one has one zero and one one, so $f(0)\ne f(1)$. The four oracles require only the following circuits:

$$
U_0=I,\qquad U_1=I\otimes X,\qquad
U_x=\operatorname{CNOT},\qquad
U_{1\oplus x}=(I\otimes X)\operatorname{CNOT}.
$$

Prepare $|0\rangle|1\rangle$, apply a [Hadamard gate](../../../../hadamard-gate.md) to each [qubit](../../../../qubit.md), apply the oracle once, apply another [Hadamard gate](../../../../hadamard-gate.md) to the first [qubit](../../../../qubit.md), and measure that first wire in the [computational basis](../../../../computational-basis.md). Immediately before the oracle the state is $|+\rangle|-\rangle$. The identity $X|-\rangle=-|-\rangle$ gives [phase kickback](../../../../phase-kickback.md):

$$
|+\rangle|-\rangle\xrightarrow{U_f}
\frac{(-1)^{f(0)}|0\rangle+(-1)^{f(1)}|1\rangle}{\sqrt2}|-\rangle
\xrightarrow{H\otimes I}
\boxed{(-1)^{f(0)}|f(0)\oplus f(1)\rangle|-\rangle.}
$$

The output is certainly zero for constant and one for balanced. In circuit terms the target $X$ contributes only a global sign, and a controlled $X$ with target $|-\rangle$ acts as $Z$ on the control; $HZH=X$ then turns that phase into a measured bit. These identities prove the network for all four explicit oracles. The unused sign contains $f(0)$ only as a global phase, consistent with the full-identification lower bound.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
