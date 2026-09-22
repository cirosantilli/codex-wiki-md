<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every $a\in\mathbb R$,

$$
X-a=(X-\mathbb EX)+(\mathbb EX-a).
$$

After squaring and taking expectations, the cross term vanishes because $\mathbb E[X-\mathbb EX]=0$. Therefore

$$
\mathbb E[(X-a)^2]
=\operatorname{Var}(X)+(\mathbb EX-a)^2.
$$

The second term is nonnegative and vanishes exactly at $a=\mathbb EX$, so the [variance as the minimum mean squared error of a constant](../../../../../../variance-as-the-minimum-mean-squared-error-of-a-constant.md) identity is

$$
\boxed{\ \operatorname{Var}(X)=\inf_{a\in\mathbb R}\mathbb E[(X-a)^2].\ }
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
