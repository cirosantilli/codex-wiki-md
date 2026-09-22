<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Split the adjacent products into two subsequences:

$$
Y_j=X_{2j-1}X_{2j},\qquad Z_j=X_{2j}X_{2j+1}\qquad(j\geq1).
$$

Within each subsequence the pairs use disjoint coordinates, so each subsequence consists of [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md). The two subsequences need not be [independent](../../../../../../independent-random-variables.md) of each other. By [independence](../../../../../../independent-random-variables.md) within a pair,

$$
\mathbb E|Y_j|=\mathbb E|Z_j|=(\mathbb E|X_1|)^2<\infty,\qquad
\mathbb E Y_j=\mathbb E Z_j=m^2.
$$

Apply the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) from (c) separately to obtain $k^{-1}\sum_{j=1}^kY_j\to m^2$ and $k^{-1}\sum_{j=1}^kZ_j\to m^2$ simultaneously [almost surely](../../../../../../almost-sure-convergence.md). Since

$$
\frac{\widetilde S_n}{n}
=\frac{\lceil n/2\rceil}{n}\frac{\sum_{j=1}^{\lceil n/2\rceil}Y_j}{\lceil n/2\rceil}
+\frac{\lfloor n/2\rfloor}{n}\frac{\sum_{j=1}^{\lfloor n/2\rfloor}Z_j}{\lfloor n/2\rfloor},
$$

and both prefactors tend to $1/2$, the [strong law for adjacent products](../../../../../../strong-law-for-adjacent-products.md) gives

$$
\boxed{\frac{\widetilde S_n}{n}\longrightarrow m^2\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
