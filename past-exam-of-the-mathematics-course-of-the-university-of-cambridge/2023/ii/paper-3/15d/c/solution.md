<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use three [controlled-NOT gates](../../../../../../controlled-not-gate.md) with control-target directions

$$
1\longrightarrow2,
\qquad
2\longrightarrow1,
\qquad
1\longrightarrow2.
$$

On computational-basis bits they act as

$$
(x,y)\longmapsto(x,x\oplus y)
\longmapsto(y,x\oplus y)
\longmapsto(y,x).
$$

They therefore implement the [Three-CNOT decomposition of the SWAP gate](../../../../../../three-cnot-decomposition-of-the-swap-gate.md), and linearity proves the identity on every two-qubit state.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
