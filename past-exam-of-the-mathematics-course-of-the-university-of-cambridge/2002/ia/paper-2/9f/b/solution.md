<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every urn contains $n-1$ balls. Let $k=n-r$ be its number of blue balls; choosing an urn uniformly makes $k$ uniform on $0,\ldots,n-1$. Conditional on that urn, the [probability](../../../../../../probability.md) of a blue first draw is $k/(n-1)$, so the [law of total probability](../../../../../../law-of-total-probability.md) gives

$$
\boxed{\mathbb P(B_1)=\frac1n\sum_{k=0}^{n-1}\frac{k}{n-1}=\frac12.}
$$

Drawing twice without replacement requires $n\ge3$. Given $k$, the [probability](../../../../../../probability.md) that both draws are blue is $k(k-1)/((n-1)(n-2))$, and hence

$$
\mathbb P(B_1\cap B_2)=\frac{\sum_{k=0}^{n-1}k(k-1)}{n(n-1)(n-2)}=\frac13.
$$

Taking the ratio defining [conditional probability](../../../../../../conditional-probability.md) gives **the second requested probability**

$$
\boxed{\mathbb P(B_2\mid B_1)=\frac{1/3}{1/2}=\frac23.}
$$

Although a blue first draw removes a blue ball from its urn, it also makes an urn rich in blue balls more likely. Averaging with this changed conditional distribution is essential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
