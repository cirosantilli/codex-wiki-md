<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For finite sets $A_1,\ldots,A_n$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\left|\bigcup_{i=1}^{n}A_i\right|
=\sum_{\varnothing\ne I\subseteq\{1,\ldots,n\}}
(-1)^{|I|+1}\left|\bigcap_{i\in I}A_i\right|.
$$

To prove it, fix an element belonging to exactly $k$ of the sets. If $k=0$, it contributes zero to both sides. If $k\geq1$, its total weight on the right is

$$
\sum_{r=1}^{k}(-1)^{r+1}\binom kr
=1-(1-1)^k=1
$$

by the [binomial theorem](../../../../../binomial-theorem.md). Summing these pointwise contributions proves the formula.

Let the universe be the $n!$ [permutations](../../../../../permutation.md) of $\{1,\ldots,n\}$, and let $A_j$ be the set of [permutations](../../../../../permutation.md) fixing $j$. A [derangement](../../../../../derangement-of-a-permutation.md) belongs to none of the $A_j$. If $k$ specified points must be fixed, the remaining $n-k$ points can be permuted in $(n-k)!$ ways, so every such $k$-fold intersection has that size. There are $\binom nk$ choices of the specified fixed points. Applying [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) to the complement of their union gives the [derangement counting formula](../../../../../derangement-counting-formula.md)

$$
\boxed{f(n)=\sum_{k=0}^{n}(-1)^k\binom nk(n-k)!
=n!\sum_{k=0}^{n}\frac{(-1)^k}{k!}.}
$$

The $k=0$ term is the whole universe. Since the exponential [power series](../../../../../power-series.md) converges absolutely at $-1$,

$$
\boxed{\lim_{n\to\infty}\frac{f(n)}{n!}
=\sum_{k=0}^{\infty}\frac{(-1)^k}{k!}=e^{-1}.}
$$

The alternating-series remainder additionally gives $\left|f(n)/n!-e^{-1}\right|\leq1/(n+1)!$. Thus the fraction is the probability of no fixed points in a uniformly chosen [permutation](../../../../../permutation.md) and approaches $1/e$.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
