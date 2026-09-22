<h1 id="31j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace the $i$th example of $D$ to obtain $D'$. The population-loss term changes by at most $\beta$ by the assumed [uniform stability of a learning algorithm](../../../../../../uniform-stability-of-a-learning-algorithm.md). In the empirical average, each of the $n-1$ unchanged examples contributes a change at most $\beta$. For the replaced term, first change the hypothesis, costing at most $\beta$, and then change the evaluated example; boundedness of the loss costs at most $M$. Thus the empirical term changes by at most

$$
\frac{(n-1)\beta+\beta+M}{n}
=\beta+\frac Mn.
$$

Combining the two terms gives

$$
\boxed{|F(D)-F(D')|\leq2\beta+\frac Mn}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
