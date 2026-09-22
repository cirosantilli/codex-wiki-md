<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The gate set is universal.** Since the [Hadamard gate](../../../../../../hadamard-gate.md) satisfies $H^\dagger=H$ and $H^2=I$, the supplied $U$ is a [unitary operator](../../../../../../unitary-operator.md), and

$$
U^2=\frac{(I-iH)^2}{2}=-iH.
$$

Two applications of $U$ therefore realize a [Hadamard gate](../../../../../../hadamard-gate.md) up to a [global phase](../../../../../../global-phase.md). Together with the supplied [controlled-NOT gate](../../../../../../controlled-not-gate.md) and [T gate](../../../../../../t-gate.md), this simulates the given [universal quantum gate set](../../../../../../universal-quantum-gate-set.md).

An exact matrix representative of $H$ can also be synthesized if desired. Put $A=U^2=-iH$ and $S=T^2$. Direct multiplication gives $(AS)^6=-iI$, hence

$$
\boxed{(AS)^{18}A=H.}
$$

This finite product uses only $U$ and $T$, so the conclusion does not rely on discarding a [global phase](../../../../../../global-phase.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
