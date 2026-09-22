<h1 id="1/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Alice cannot send a [bit](../../../../../../bit.md) to Charlie either.** An argument based only on the apparent chronological chain would be insufficient: Alice interacts with Bob before Bob interacts with Charlie. The extra fact is that these particular gates commute.

In Bob's [computational basis](../../../../../../computational-basis.md) the complete gate is

$$
U=I_A\otimes|0\rangle\langle0|_B\otimes I_C
+X_A\otimes|1\rangle\langle1|_B\otimes X_C.
$$

Both [controlled-NOT gates](../../../../../../controlled-not-gate.md) preserve Bob's control label, and their target operations act on different systems. Thus $WV=VW$. We may consequently regard Bob–Charlie as the first interaction and Bob–Alice as the last one. The final operation on $AB$ cannot change Charlie's [reduced density matrix](../../../../../../reduced-density-matrix.md), and Charlie's earlier state cannot depend on Alice's initially separate preparation.

The [target no-signalling in a common-control unitary](../../../../../../target-no-signalling-in-a-common-control-unitary.md) formula makes the independence explicit:

$$
\boxed{\rho_C'=\langle0|\rho_B|0\rangle\rho_C
+\langle1|\rho_B|1\rangle X\rho_CX.}
$$

Alice's [density matrix](../../../../../../density-matrix-split.md) does not appear. The formula includes arbitrary complex initial amplitudes and every final measurement on Charlie. This conclusion uses the specified pair of gates; a general intervening operation on Bob could change the communication possibilities.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
