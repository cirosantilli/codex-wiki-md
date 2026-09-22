<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [superdense coding](../../../../superdense-coding.md), Alice and Bob initially share $|\Psi^+\rangle_{AB}$. Alice selects the same one-qubit [Pauli gate](../../../../pauli-gate.md) $I,Z,X,XZ$ according to her message and sends her single encoded [qubit](../../../../qubit.md) to Bob. He now has both halves and measures in the [Bell basis](../../../../bell-basis.md). For the chosen assignment,

$$
\boxed{\Pr(Y=j\mid X=i)=\delta_{ij},\qquad I(X:Y)=H(X),}
$$

which reaches two bits for the uniform distribution. A circuit implementation first converts the resource convention with $X_B$, then applies $\operatorname{CNOT}_{A\to B}$ and $H_A$, and measures both in the [computational basis](../../../../computational-basis.md). The four outcomes are distinct; relabeling them restores the selected message order.

Before Alice's transmission, Bob's reduced [density operator](../../../../density-matrix-split.md) is $I/2$ for every choice of her local operation. Thus distributing the message-independent entangled resource has transmitted no information about the subsequently chosen message. It is nevertheless a real physical resource: the two-bit rate counts the one additional transmitted [qubit](../../../../qubit.md) after entanglement has been shared, not a free initial distribution. The deterministic conditional probabilities above establish perfect correlation rather than merely matching output and input entropies.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
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
