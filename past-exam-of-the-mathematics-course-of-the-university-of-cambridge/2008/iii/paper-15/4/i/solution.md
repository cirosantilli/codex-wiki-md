<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $X$ uniformly among the $n$ vertices. For each covering graph use a proper binary coloring, and fill the color of an absent vertex with an independent random color having the same law as the color of a uniform vertex of that graph, as in the question's construction. Write $h_i$ for that color [information entropy](../../../../../../information-entropy.md), so $h_i\leq1$. The marginal distribution of $Y_i$ is precisely this color law, and the variables $Y_i$ are conditionally independent given $X$: present colors are deterministic and absent colors use independent dummy draws. Therefore

$$
H(Y_1,\ldots,Y_\ell\mid X)=\sum_i(1-|G_i|/n)h_i,\qquad H(Y_1,\ldots,Y_\ell)\leq\sum_i h_i.
$$

Any two distinct vertices are joined in some $G_i$ and have different forced colors there. They cannot both be compatible with the same observed color vector, so $H(X\mid Y_1,\ldots,Y_\ell)=0$. The [mutual information](../../../../../../mutual-information.md) identity now gives

$$
\log_2n\leq\frac1n\sum_i|G_i|h_i\leq\frac1n\sum_i|G_i|,
$$

and hence $\boxed{\sum_i|G_i|\geq n\log_2n}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
