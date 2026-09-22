<h1 id="b/4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $X_k=\sum_iI_i$. For two disjoint blocks, their relative orders are independent and each is increasing with [probability](../../../../../../probability.md) $1/k!$, giving joint [probability](../../../../../../probability.md) $1/(k!)^2$. If their cyclic starting positions differ by $s$, with $1\leq s<k$, and $k\leq n/2$, they overlap in just one interval. Both blocks increasing is then equivalent to their entire length-$k+s$ union increasing, so the joint [probability](../../../../../../probability.md) is $1/(k+s)!$.

For each $s$ there are $2n$ ordered overlapping pairs, while there are $n(n-2k+1)$ ordered disjoint pairs and $n$ diagonal pairs. Thus for $k\geq2$,

$$
\mathbb EX_k^2=\frac n{k!}+2n\sum_{s=1}^{k-1}\frac1{(k+s)!}+\frac{n(n-2k+1)}{(k!)^2}.
$$

The tail is bounded using $(k+s)!\geq k!(k+1)^s$:

$$
\sum_{s=1}^{k-1}\frac1{(k+s)!}\leq\frac1{k!}\sum_{s\geq1}(k+1)^{-s}=\frac1{k\,k!}\leq\frac1{2k!}.
$$

Dropping the negative correction in the disjoint term proves

$$
\boxed{\mathbb EX_k^2\leq\frac{n^2}{(k!)^2}+\frac{2n}{k!}}.
$$

For $k=1$, $X_1=n$ deterministically and the same bound is immediate.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
