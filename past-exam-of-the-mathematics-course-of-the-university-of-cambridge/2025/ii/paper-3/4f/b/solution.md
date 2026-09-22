<h1 id="4f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the same program as $N$, replacing only its first line by a test for a final $1$:

$$
\begin{array}{c|l}
q_S&\mapsto ?_1(0,q_3,q_0)\\
q_0&\mapsto -(0,q_2,q_0)\\
q_1&\mapsto +_1(0,q_H)\\
q_2&\mapsto +_0(0,q_H)\\
q_3&\mapsto -(0,q_1,q_3)\\
q_H&\mapsto ?_\varepsilon(0,q_H,q_H).
\end{array}
$$

If the input ends in $1$, the $q_3$ loop erases it and eventually appends output $1$. Every other input, including the empty word, follows the $q_0$ loop and produces $0$. This is the characteristic function of $\{w1:w\in\mathbb B\}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4F](../../4f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
