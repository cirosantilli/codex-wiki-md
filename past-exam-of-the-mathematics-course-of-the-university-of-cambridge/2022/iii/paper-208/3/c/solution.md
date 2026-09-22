<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B$ be the set of bins that are occupied in configuration $x$ but empty in configuration $y$. For each $b\in B$, choose the lowest-numbered ball $j_b$ lying in $b$ under $x$. Then $\alpha_{j_b}(x)=1$ and $x_{j_b}\ne y_{j_b}$. Distinct bins choose distinct balls, so

$$
|B|\leq\sum_{j=1}^m\alpha_j(x)\mathbf1_{\{x_j\ne y_j\}}.
$$

Every increase in the number of empty bins is accounted for by a newly empty bin, while newly occupied bins only decrease that number. Hence $f(y)-f(x)\leq|B|$, proving the stated inequality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
