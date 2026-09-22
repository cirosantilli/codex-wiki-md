<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the known [phase gate](../../../../../../../phase-gate.md) on the answer register be

$$
P|y\rangle=(-1)^{[y^4\leq N]}|y\rangle,
$$

where the comparison uses ordinary [integers](../../../../../../../integer.md), not [modular arithmetic](../../../../../../../modular-arithmetic.md). A [reversible circuit](../../../../../../../reversible-circuit.md) computes the predicate, applies a [Pauli Z gate](../../../../../../../pauli-z-gate.md) to its flag, then performs [uncomputation](../../../../../../../uncomputation.md).

The [compute-phase-uncompute construction](../../../../../../../compute-phase-uncompute-construction.md) now gives

$$
|x,0\rangle\xrightarrow{U_f}|x,f(x)\rangle
\xrightarrow{I\otimes P}(-1)^{[f(x)^4\leq N]}|x,f(x)\rangle
\xrightarrow{U_f^{-1}}(-1)^{[f(x)^4\leq N]}|x,0\rangle.
$$

Use [modular-oracle inversion by negation](../../../../../../../modular-oracle-inversion-by-negation.md) to realize the last operation with one further $U_f$ query. **Exactly two oracle queries implement $I_g$, returning the answer register and comparison workspace to their initial states.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
