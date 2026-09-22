<h1 id="15c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three [controlled-NOT gates](../../../../../../controlled-not-gate.md) have directions $1\to2$, $2\to1$, and $1\to2$. On [computational basis](../../../../../../computational-basis.md) bits they act as

$$
(x,y)\mapsto(x,x\oplus y)
\mapsto(y,x\oplus y)
\mapsto(y,x).
$$

By linearity, the whole [quantum circuit](../../../../../../quantum-circuit-split.md) is the [SWAP gate](../../../../../../swap-gate.md). Therefore

$$
\boxed{U(|\psi\rangle\otimes|\phi\rangle)
=|\phi\rangle\otimes|\psi\rangle},
$$

so $|\alpha\rangle=|\phi\rangle$ and $|\beta\rangle=|\psi\rangle$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15C](../../15c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
