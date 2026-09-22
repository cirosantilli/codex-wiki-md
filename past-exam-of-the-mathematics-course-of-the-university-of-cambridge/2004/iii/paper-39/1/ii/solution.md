<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [law of total variance](../../../../../../law-of-total-variance.md) to each epoch. The [Poisson distribution](../../../../../../poisson-distribution.md) has equal conditional mean and [variance](../../../../../../variance-split.md), while $\operatorname{Var}(T_j)=\binom j2^{-2}$. Hence

$$
\operatorname{Var}(Y_j)=\mathbb E\!\left[\frac{j\theta T_j}{2}\right]+\operatorname{Var}\!\left(\frac{j\theta T_j}{2}\right)=\frac{\theta}{j-1}+\frac{\theta^2}{(j-1)^2}.
$$

The [independent mutation counts in coalescent epochs](../../../../../../independent-mutation-counts-in-coalescent-epochs.md) permit [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md). Thus

$$
\boxed{\operatorname{Var}(S)=\theta H_{n-1}+\theta^2H_{n-1}^{(2)},\qquad H_{n-1}^{(2)}=\sum_{i=1}^{n-1}\frac1{i^2}.}
$$

The first term is conditional [Poisson distribution](../../../../../../poisson-distribution.md) variation; the second comes from the random lengths of the ancestral tree. These are the [moments of the mutation count on a neutral coalescent tree](../../../../../../moments-of-the-mutation-count-on-a-neutral-coalescent-tree.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
