<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Track the $-i$ factors only when the corresponding transition is addressed. They are common within the addressed two-state subspace, but become physically relevant relative [phases](../../../../phase-waves.md) between computational [basis](../../../../basis.md) states. Using a semicolon to separate the shared motional [number state](../../../../number-state.md), the complete paths are

$$
\begin{aligned}
|gg;0\rangle&\longrightarrow|gg;0\rangle\longrightarrow|gg;0\rangle\longrightarrow|gg;0\rangle,\\
|ge;0\rangle&\longrightarrow|ge;0\rangle\longrightarrow|ge;0\rangle\longrightarrow|ge;0\rangle,\\
|eg;0\rangle&\longrightarrow-i|gg;1\rangle\longrightarrow-i|gg;1\rangle\longrightarrow-|eg;0\rangle,\\
|ee;0\rangle&\longrightarrow-i|ge;1\rangle\longrightarrow+i|ge;1\rangle\longrightarrow|ee;0\rangle.
\end{aligned}
$$

The middle arrow comprises both Y pulses. In the last row those individual steps are $-i|ge;1\rangle\to-|gf;0\rangle\to+i|ge;1\rangle$. The two X pulses contribute $(-i)^2=-1$ for either initially excited control; the Y pair supplies a second minus sign only when the second ion is also excited.

The shared motion returns to its [ground state](../../../../ground-state.md) for all four inputs, and the auxiliary internal state is empty. [Quantum superposition](../../../../quantum-superposition.md) therefore gives the [two-qubit gate](../../../../two-qubit-gate.md)

$$
\boxed{G=\operatorname{diag}(1,1,-1,1)=Z_a C_Z,\qquad
C_Z=\operatorname{diag}(1,1,1,-1).}
$$

Discarding the X-pulse factors would incorrectly identify $G$ with a [Controlled-Z gate](../../../../controlled-z-gate.md) itself.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
