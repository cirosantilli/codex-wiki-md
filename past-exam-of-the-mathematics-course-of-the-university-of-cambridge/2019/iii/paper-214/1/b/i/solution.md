<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
a_n=-\log\mathbb P_p(0\leftrightarrow e_n).
$$

The events $\{0\leftrightarrow e_n\}$ and $\{e_n\leftrightarrow e_{n+m}\}$ are increasing events of [bond percolation](../../../../../../../bond-percolation-split.md). The [FKG inequality](../../../../../../../fkg-inequality.md) and translation invariance give

$$
\mathbb P_p(0\leftrightarrow e_{n+m})
\geq \mathbb P_p(0\leftrightarrow e_n)
\mathbb P_p(e_n\leftrightarrow e_{n+m})
=\mathbb P_p(0\leftrightarrow e_n)
\mathbb P_p(0\leftrightarrow e_m).
$$

Thus $(a_n)$ is a [subadditive sequence](../../../../../../../subadditive-sequence.md). Since every probability is positive for $p>0$, [Fekete lemma](../../../../../../../fekete-s-lemma.md) applies and gives

$$
\boxed{\phi(p)=\lim_{n\to\infty}a_n/n
=\inf_{n\geq1}\left[-\frac1n\log\mathbb P_p(0\leftrightarrow e_n)\right].}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
