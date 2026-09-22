<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

If $\mathcal G\subseteq\mathcal H$, then $\mathbb E[X\mid\mathcal G]$ is already $\mathcal H$-measurable, so

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal G]
=\mathbb E[X\mid\mathcal G\cap\mathcal H].
$$

If $\mathcal H\subseteq\mathcal G$, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H]
=\mathbb E[X\mid\mathcal G\cap\mathcal H].
$$

Finally, if $\mathcal G$ and $\mathcal H$ are independent, the $\mathcal G$-measurable variable $\mathbb E[X\mid\mathcal G]$ is independent of $\mathcal H$. Its conditional expectation given $\mathcal H$ is its mean $\mathbb E[X]$. Part c shows that the right side is also $\mathbb E[X]$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
