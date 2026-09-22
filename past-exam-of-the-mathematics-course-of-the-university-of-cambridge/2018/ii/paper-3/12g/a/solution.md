<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) states that for every [regular language](../../../../../../regular-language.md) $L$ there is an integer $N$ such that every $w\in L$ with $|w|\geq N$ can be written

$$
w=xyz
$$

with

$$
|xy|\leq N,\qquad |y|\geq1,\qquad
xy^rz\in L\quad\text{for every }r\geq0.
$$

To prove it, let a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) with $N$ states recognize $L$. During the reading of the first $N$ symbols of an accepted word $w$, the automaton visits $N+1$ states, including the initial state. By the [pigeonhole principle](../../../../../../pigeonhole-principle.md), two of them agree, say $q_i=q_j$ with $0\leq i<j\leq N$. Let $x$ be the first $i$ symbols, $y$ the next $j-i$ symbols, and $z$ the remaining suffix. Reading $y$ is a nonempty closed path from $q_i$ to itself. Traversing this path any number $r\geq0$ of times and then reading $z$ therefore reaches the same accept state. This proves all three assertions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
