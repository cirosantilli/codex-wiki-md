<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a,b$ be as in [i](../b/i.md). Insert the explicit [oracle](../../../../boolean-quantum-oracle.md) from [ii](../b/ii.md) between the two pairs of [Hadamard gates](../../../../hadamard-gate.md). The network identities

$$
HXH=Z,\qquad
(H\otimes H)\operatorname{CNOT}_{x\to y}(H\otimes H)
=\operatorname{CNOT}_{y\to x}
$$

turn the entire network into

$$
U_D=(I\otimes Z^a)\operatorname{CNOT}_{y\to x}^{\,b}.
$$

This is the last simplified circuit in [i](../../4/b/i.md). On the designated input $|0\rangle_x|1\rangle_y$, its reversed control is certainly one, so

$$
\boxed{U_D|0,1\rangle=(-1)^a|b,1\rangle
=(-1)^{f(0)}|f(0)\oplus f(1),1\rangle.}
$$

The [global phase](../../../../global-phase.md) is unobservable. Measuring the first wire therefore determines the function class with certainty after one [oracle](../../../../boolean-quantum-oracle.md) query, while the second wire returns to $|1\rangle$. These circuit identities are the network form of [quantum phase kickback](../../../../phase-kickback.md): the answer state between the Hadamards is the $X$ [eigenstate](../../../../eigenstate.md) $|-\rangle$, on which an [XOR](../../../../exclusive-or.md) acts as a phase.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
