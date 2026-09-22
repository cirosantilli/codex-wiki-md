<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $\tau_0=0$ and apply part c recursively. A lazy walk makes a genuine jump with probability $1/2$, so the expected time required for $2j$ jumps is $4j$. Using the stated independence,

$$
\mathbb E_0\tau_k
=4\mathbb E_0\tau_{k-1}+1.
$$

The initial value zero solves this recurrence as

$$
\boxed{\mathbb E_0\tau_k=\frac{4^k-1}{3}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
