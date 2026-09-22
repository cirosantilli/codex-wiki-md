<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split a [self-avoiding walk](../../../../../../self-avoiding-walk.md) of length $m+n$ after its first $m$ steps. Its prefix is one of the $c_m$ walks, and its translated suffix is a [self-avoiding walk](../../../../../../self-avoiding-walk.md) of length $n$ from the origin. The pair determines the original walk, although not every pair can be concatenated without intersection. Therefore

$$
c_{m+n}\le c_mc_n.
$$

All $c_n$ are positive, so $x_n=\log c_n$ is a [subadditive sequence](../../../../../../subadditive-sequence.md). The [Fekete lemma](../../../../../../fekete-s-lemma.md) gives existence of $\lim_n n^{-1}\log c_n$ and consequently of the [connective constant](../../../../../../connective-constant.md).

For a lower bound, all words of length $n$ using only north and east steps produce distinct [self-avoiding walks](../../../../../../self-avoiding-walk.md): the sum of the two coordinates increases at each step. Thus $c_n\ge2^n$. For an upper bound, there are four choices for the first step and at most three thereafter, since a [self-avoiding walk](../../../../../../self-avoiding-walk.md) cannot immediately reverse its previous [edge](../../../../../../edge-of-a-graph.md). Hence $c_n\le4\,3^{n-1}$. Taking $n$th roots proves

$$
\boxed{\kappa=\lim_{n\to\infty}c_n^{1/n}
=\inf_{n\ge1}c_n^{1/n},\qquad 2\le\kappa\le3.}
$$

The elementary upper bound counts all non-backtracking walks, including some that self-intersect, so it is an upper estimate rather than an equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
