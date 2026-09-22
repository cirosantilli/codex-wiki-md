<h1 id="4h/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [bounded-run deterministic finite automaton](../../../../../../../bounded-run-deterministic-finite-automaton.md) with states

$$
q_0,q_1,\ldots,q_7,q_{\rm dead}.
$$

State $q_j$ records that the current suffix consists of exactly $j$ consecutive zeros. Every $q_0,\ldots,q_7$ is accepting; $q_{\rm dead}$ is rejecting. Reading $1$ sends every accepting state to $q_0$, while reading $0$ sends $q_j$ to $q_{j+1}$ for $j<7$ and sends $q_7$ to $q_{\rm dead}$. The dead state loops on both symbols. This finite automaton accepts exactly the words with no run of eight zeros, so

$$
\boxed{\text{the language is regular}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4H](../../../4h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
