<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [no-cloning theorem](../../../../no-cloning-theorem.md) states that no fixed deterministic [quantum operation](../../../../quantum-operation.md) can perfectly duplicate every unknown [pure state](../../../../pure-state.md). For a [unitary](../../../../unitary-connection.md) copier with a fixed blank, suppose it cloned two normalized vectors $|a\rangle,|b\rangle$. Preservation of [inner products](../../../../inner-product-split.md) would give $\langle a|b\rangle=\langle a|b\rangle^2$, impossible for a nonorthogonal distinct pair with overlap strictly between zero and one in modulus. Including an environment does not help: its final overlap has modulus at most one, so one would require $|\langle a|b\rangle|\leq|\langle a|b\rangle|^2$. Thus a universal perfect copier is impossible. [Orthogonal](../../../../orthogonal-vectors.md) known alternatives do not contradict this restriction.

Label the three [qubits](../../../../qubit.md) as input $S$, Alice's entangled [qubit](../../../../qubit.md) $A$ and Bob's [qubit](../../../../qubit.md) $B$. Initially their joint state is

$$
\frac1{\sqrt2}[\alpha_0(|000\rangle+|011\rangle)+\alpha_1(|100\rangle+|111\rangle)].
$$

The [controlled-NOT gate](../../../../controlled-not-gate.md) from $S$ to $A$ changes this to

$$
\frac1{\sqrt2}[\alpha_0(|000\rangle+|011\rangle)+\alpha_1(|110\rangle+|101\rangle)].
$$

Apply $H|0\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $H|1\rangle=(|0\rangle-|1\rangle)/\sqrt2$ to the first [qubit](../../../../qubit.md) and group by Alice's two computational-basis outcomes. The result is

$$
\boxed{\frac12\bigl[|00\rangle|\psi\rangle+|01\rangle X|\psi\rangle+
|10\rangle Z|\psi\rangle+|11\rangle XZ|\psi\rangle\bigr].}
$$

In expanded form the last two Bob factors are $\alpha_0|0\rangle-\alpha_1|1\rangle$ and $\alpha_0|1\rangle-\alpha_1|0\rangle$. **Their Alice labels must be $10$ and $11$; the repeated $00$ labels in the source are printing errors.**

Alice measures her two [qubits](../../../../qubit.md) and sends the two classical bits $(a,b)$ to Bob. Each outcome has probability $1/4$ and Bob's conditional state is $X^bZ^a|\psi\rangle$. He applies $\boxed{Z^aX^b}$ to recover the input, up to physically irrelevant [global phase](../../../../global-phase.md). Explicitly the corrections for $00,01,10,11$ are $I,X,Z,ZX$. This is [quantum teleportation](../../../../quantum-teleportation.md): Alice's input is consumed by [measurement](../../../../measurement.md), so no second surviving copy is created. Before her classical message, Bob's [reduced density operator](../../../../reduced-density-matrix.md) is $I/2$, independent of the input, so the protocol also supplies no faster-than-light communication.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
