<h1 id="12j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The upper register index is the largest register number occurring in an instruction of $P$, with value zero if only register $0$ is used. A configuration records the current state and the contents of every register up to that index.

For input $\vec w$, let $C(0,M,\vec w)$ be the initial configuration: the designated initial state, the words of $\vec w$ in the input registers, and the empty word in every remaining register. Recursively, if $C(t,M,\vec w)$ is halting, keep it fixed; otherwise let $C(t+1,M,\vec w)$ be the unique configuration into which $M$ transforms it. The resulting [sequence](../../../../../../sequence.md)

$$
\boxed{\{C(t,M,\vec w):t\in\mathbb N\}}
$$

is the computation [sequence](../../../../../../sequence.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12J](../../12j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
