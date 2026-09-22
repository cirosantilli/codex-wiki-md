<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $|\alpha|^2+|\beta|^2=1$. Let Alice's first recorded [quantum measurement](../../../../quantum-measurement-split.md) outcome be $a\in\{0,1\}$. Immediately afterward she assigns the conditional [pure quantum state](../../../../pure-state.md) $|a\rangle$, with probabilities $p_0=|\alpha|^2$, $p_1=|\beta|^2$. Bob, who has no record, assigns the [density operator](../../../../density-matrix-split.md)

$$
\boxed{\rho_{B,1}=|\alpha|^2|0\rangle\langle0|+|\beta|^2|1\rangle\langle1|.}
$$

This is a [nonselective quantum measurement](../../../../nonselective-quantum-measurement.md), which removes the initial [computational basis](../../../../computational-basis.md) coherence. It is not generally the original [pure quantum state](../../../../pure-state.md).

After the [Hadamard gate](../../../../hadamard-gate.md), Alice assigns $H|a\rangle=|+\rangle$ for $a=0$, or $|-\rangle$ for $a=1$. Bob assigns

$$
H\rho_{B,1}H=|\alpha|^2|+\rangle\langle+|+|\beta|^2|-\rangle\langle-|.
$$

Both $|+\rangle$ and $|-\rangle$ give either final [computational basis](../../../../computational-basis.md) outcome with [probability](../../../../probability.md) $1/2$. Thus, after Alice records the second outcome $b$, she assigns $|b\rangle$, whereas Bob assigns

$$
\boxed{\rho_{B,2}=\tfrac12|0\rangle\langle0|+\tfrac12|1\rangle\langle1|=I/2.}
$$

Alice's conditional [quantum states](../../../../quantum-state.md) are pure; Bob's are averages over her unobserved records. They agree on all probabilities when supplied the same information. Their first descriptions can coincide if the initial [quantum state](../../../../quantum-state.md) is a [computational basis](../../../../computational-basis.md) state; after the second [quantum measurement](../../../../quantum-measurement-split.md), Bob's [maximally mixed state](../../../../maximally-mixed-state.md) differs from each conditional [pure quantum state](../../../../pure-state.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
