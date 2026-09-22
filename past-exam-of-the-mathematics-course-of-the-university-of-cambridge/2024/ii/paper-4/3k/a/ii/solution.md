<h1 id="3k/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The unicity distance is the least ciphertext length for which the key is determined, or in the usual approximation the length at which the expected number of spurious keys falls to about zero. Assume equiprobable keys, a stationary plaintext source of [information entropy](../../../../../../../information-entropy.md) rate $H_E$, and ciphertext symbols that are approximately uniform on $A$. The language redundancy per symbol is

$$
D=\log_2|A|-H_E.
$$

The key equivocation is then approximated by

$$
H(K\mid C_1,ldots,C_n)\simeq\log_2|K|-nD.
$$

Hence the classical closed-form estimate is

$$
\boxed{n_0\simeq\frac{\log_2|K|}{\log_2|A|-H_E}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3K](../../../3k.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
