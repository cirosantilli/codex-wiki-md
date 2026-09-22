<h1 id="10c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $x=x_1x_2$. Since the marked word is $11$, the required oracle is a single [Toffoli gate](../../../../../../toffoli-gate.md) with $x_1$ and $x_2$ as its two controls and the answer qubit $y$ as its target:

$$
|x_1x_2\rangle|y\rangle
\longmapsto
|x_1x_2\rangle|y\mathbin\oplus(x_1x_2)\rangle.
$$

The target flips exactly when both controls are one, which is exactly when $x=11$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10C](../../10c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
