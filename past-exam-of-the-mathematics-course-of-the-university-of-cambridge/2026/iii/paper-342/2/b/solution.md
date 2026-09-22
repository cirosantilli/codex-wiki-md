<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The six displayed generators of the [Steane code](../../../../../../steane-code.md) are independent and commuting, so the common positive eigenspace has dimension

$$
2^{7-6}=2;
$$

it encodes one logical qubit. The binary columns of the underlying Hamming parity-check matrix are all nonzero and distinct. Hence no weight-one or weight-two Pauli lies in the stabilizer normalizer outside the stabilizer. On the other hand,

$$
\overline X=X_1X_2\cdots X_7
$$

is logical, and multiplying it by $X_1X_2X_3X_4$ gives the weight-three representative

$$
\overline X\sim X_5X_6X_7.
$$

The analogous statement holds for $\overline Z$, so

$$
\boxed{d=3}.
$$

Now include both $E_1=X_5$ and $E_2=X_6X_7$ in the proposed error set. Their product is

$$
E_1^\dagger E_2=X_5X_6X_7\sim\overline X,
$$

which is non-scalar on the code and violates the [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md). Since multiplying by a logical operator does not change commutation with stabilizers, $X_5$ and $X_6X_7$ have the same [error syndrome](../../../../../../error-syndrome.md). A decoder cannot know which occurred and may apply a correction that leaves a logical $\overline X$ error.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
