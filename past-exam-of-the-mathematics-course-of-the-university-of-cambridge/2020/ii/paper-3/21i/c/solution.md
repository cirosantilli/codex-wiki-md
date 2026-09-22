<h1 id="21i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $E=\operatorname{im}S$, a finite-dimensional subspace, and decompose $H=E\oplus E^\perp$. The restriction

$$
(S-\lambda I)|_E:E\to E
$$

is injective, because a nonzero vector in its kernel would be a $\lambda$-eigenvector of $S$. By finite-dimensionality it is therefore surjective.

Given $y=y_E+y_\perp$, first put $x_\perp=-y_\perp/\lambda$. Then $Sx_\perp\in E$, so choose $x_E\in E$ such that

$$
(S-\lambda I)x_E=y_E-Sx_\perp.
$$

For $x=x_E+x_\perp$ we obtain $(S-\lambda I)x=y$. Hence $S-\lambda I$ is surjective. This is the [finite-rank Fredholm alternative](../../../../../../finite-rank-fredholm-alternative.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21I](../../21i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
