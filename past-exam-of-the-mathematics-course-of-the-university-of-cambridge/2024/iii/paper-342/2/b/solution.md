<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Measure each generator $S_j$. If a Pauli error $E$ has occurred, its outcome is $(-1)^{s_j}$, where

$$
S_jE=(-1)^{s_j}ES_j,
\qquad s_j\in\{0,1\}.
$$

The bit vector $s=(s_1,\ldots,s_m)$ is the [error syndrome](../../../../../../error-syndrome.md). Choose one representative $E_s$ with this syndrome. Another Pauli $E$ has the same syndrome exactly when $E_s^\dagger E$ commutes with every $S_j$, namely when $E_s^\dagger E\in C(S)$. Therefore

$$
E\in E_sC(S).
$$

This [stabilizer-syndrome coset](../../../../../../stabilizer-syndrome-coset.md) is all the syndrome reveals: multiplication by a stabilizer changes nothing on the code, while multiplication by an element of $C(S)\setminus S$ can change the logical state without changing any syndrome bit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
