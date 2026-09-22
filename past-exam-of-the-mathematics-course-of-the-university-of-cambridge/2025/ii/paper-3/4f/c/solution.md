<h1 id="4f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rename the old halt state $q_H$ as a nonhalting state $q_F$, including every occurrence of $q_H$ in the original program, and introduce a new halt state $q_H$. Attach the following output-flipping routine:

$$
\begin{array}{c|l}
q_F&\mapsto ?_0(0,q_{0},q_{1})\\
q_{0}&\mapsto -(0,q_{+1},q_{+1})\\
q_{1}&\mapsto -(0,q_{+0},q_{+0})\\
q_{+1}&\mapsto +_1(0,q_H)\\
q_{+0}&\mapsto +_0(0,q_H)\\
q_H&\mapsto ?_\varepsilon(0,q_H,q_H).
\end{array}
$$

Because the original machine computes a characteristic function, it reaches $q_F$ with register $0$ containing exactly $0$ or $1$. The routine tests that symbol, removes it, and appends its complement. It therefore halts with $1-\chi_X(w)=\chi_{\mathbb B\setminus X}(w)$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
