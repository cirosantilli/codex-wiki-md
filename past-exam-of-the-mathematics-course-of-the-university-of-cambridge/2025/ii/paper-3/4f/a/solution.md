<h1 id="4f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The instruction $-(0,p,q)$ goes to $p$ if register $0$ is empty; otherwise it deletes the final letter and goes to $q$.

For $M$, an empty input goes directly from $q_S$ to $q_1$, where a $1$ is appended. On a nonempty input, state $q_0$ deletes every letter; once the register is empty it goes to $q_2$ and appends $0$. Hence

$$
A=\{\varepsilon\}.
$$

For $N$, the initial instruction tests whether the final letter is $0$. If it is, state $q_3$ deletes the entire word and then goes to $q_1$, producing $1$. Otherwise state $q_0$ deletes the entire word and goes to $q_2$, producing $0$. Thus

$$
B=\{w0:w\in\mathbb B\},
$$

the set of nonempty binary words ending in $0$.

## ↑ Ancestors (11)

1. [A](../a.md)
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
