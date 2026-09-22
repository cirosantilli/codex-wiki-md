<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives

$$
\boxed{\mathbb P\left(\bigcup_{i=1}^nA_i\right)=
\sum_{\varnothing\ne I\subseteq\{1,\ldots,n\}}(-1)^{|I|+1}\mathbb P\left(\bigcap_{i\in I}A_i\right).}
$$

For the coat problem, all $n!$ [permutations](../../../../../permutation.md) are equally likely. If a specified set of $j$ people gets its own coats, the other coats can be assigned in $(n-j)!$ ways, so that intersection has [probability](../../../../../probability.md) $(n-j)!/n!$. Taking the complement of the union of correct-coat events gives the [derangement](../../../../../derangement-of-a-permutation.md) [probability](../../../../../probability.md)

$$
\boxed{p(0,n)=\sum_{j=0}^n\frac{(-1)^j}{j!}.}
$$

To have exactly $m$ fixed coats, choose their recipients and derange all remaining coats. Thus the [fixed point count of a uniform random permutation](../../../../../fixed-point-count-of-a-uniform-random-permutation.md) has

$$
\boxed{p(m,n)=\frac{\binom nmD_{n-m}}{n!}
=\frac{p(0,n-m)}{m!}
=\frac1{m!}\sum_{j=0}^{n-m}\frac{(-1)^j}{j!},\quad0\le m\le n,}
$$

and zero [probability](../../../../../probability.md) outside this range. The empty [permutation](../../../../../permutation.md) has $D_0=1$, so the formula includes $m=n$; it also gives zero for $m=n-1$, since a lone remaining coat cannot be misplaced.

For fixed $m$, $n-m\to\infty$, and the exponential series gives

$$
\boxed{\lim_{n\to\infty}p(m,n)=\frac{e^{-1}}{m!}.}
$$

These are the [probabilities](../../../../../probability.md) of a [Poisson distribution](../../../../../poisson-distribution.md) of [mean](../../../../../expected-value.md) one. The limit is for fixed $m$, not for $m$ increasing with $n$.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
