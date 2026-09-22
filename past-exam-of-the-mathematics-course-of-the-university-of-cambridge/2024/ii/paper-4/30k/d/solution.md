<h1 id="30k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For hinge loss, choose

$$
t_i=y_is_i,
\qquad
s_i=\begin{cases}
1,&y_ix_i^T\widehat\beta<1,\\
0,&y_ix_i^T\widehat\beta>1,\\
\text{any value in }[0,1],&y_ix_i^T\widehat\beta=1.
\end{cases}
$$

The subgradient optimality condition is

$$
0=-\frac1nX^Tt+2\lambda X^T\widehat\alpha.
$$

Injectivity of $X^T$ gives $t/n=2\lambda\widehat\alpha$. Multiplying by $XX^T$ and writing $k_i$ for its $i$th column yields

$$
\frac1n\sum_i k_it_i=2\lambda XX^T\widehat\alpha.
$$

If $y_ix_i^T\widehat\beta>1$, then $t_i=0$, and $t/n=2\lambda\widehat\alpha$ implies $\widehat\alpha_i=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30K](../../30k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
