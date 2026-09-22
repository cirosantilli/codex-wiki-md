<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [entanglement-assisted promised equality protocol](../../../../../entanglement-assisted-promised-equality-protocol.md). Alice applies the [phase oracle](../../../../../phase-oracle.md) $O_x|i\rangle=(-1)^{x_i}|i\rangle$ on $A$, and Bob applies $O_y|i\rangle=(-1)^{y_i}|i\rangle$ on $B$. These are [unitary operators](../../../../../unitary-operator.md) because their diagonal entries have [modulus](../../../../../modulus.md) one. After Alice sends $A$ to Bob, the joint [pure state](../../../../../pure-state.md) is

$$
|\Omega_{xy}\rangle=\frac1{\sqrt n}\sum_{i=0}^{n-1}(-1)^{x_i+y_i}|ii\rangle.
$$

Let $|\Omega\rangle=n^{-1/2}\sum_i|ii\rangle$ be the original [maximally entangled state](../../../../../maximally-entangled-state.md). If $d=d_H(x,y)$ is the [Hamming distance](../../../../../hamming-distance.md), then

$$
\langle\Omega|\Omega_{xy}\rangle
=\frac1n\sum_i(-1)^{x_i+y_i}
=\frac{n-d-d}{n}=1-\frac{2d}{n}.
$$

Bob performs the [projective measurement](../../../../../projective-measurement.md) with projectors $P=|\Omega\rangle\langle\Omega|$ and $I-P$. Under the promise,

$$
\boxed{d=0\implies\Pr(P)=1,\qquad
d=n/2\implies\Pr(P)=0.}
$$

He declares equal strings for the first outcome and distance $n/2$ for the other. This is exact because the promised outputs occupy [orthogonal](../../../../../orthogonal-vectors.md) subspaces. A [basic measurement](../../../../../basic-measurement.md) also suffices: extend $|\Omega\rangle$ to an [orthonormal basis](../../../../../orthonormal-basis.md) and group all its other outcomes together. Alice transmits one $n$-dimensional system, realizable using $\lceil\log_2n\rceil$ [qubits](../../../../../qubit.md); $n$ need not be a power of two.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
