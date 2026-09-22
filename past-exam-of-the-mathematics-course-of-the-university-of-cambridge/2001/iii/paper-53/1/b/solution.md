<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [interval exactness of a tent-map core](../../../../../../interval-exactness-of-a-tent-map-core.md) from the preceding part. Choose two separated nondegenerate [closed intervals](../../../../../../closed-real-interval.md) $J_0,J_1$ inside $J=(1-s,1)$. There are integers $n_i$ with $T_s^{n_i}(J_i)=A$. Taking $N=\max(n_0,n_1)$ works for both, because $T_s(A)=A$:

$$
F(J_0)=F(J_1)=A,\qquad F=T_s^N.
$$

Within each $J_i$, the [continuous function](../../../../../../continuous-function.md) $F$ attains both endpoint levels $1-s$ and $1$. Choose a segment between those levels, reversing its orientation if necessary. Starting from a point at level $1-s$, take the first point at level one, and then the last point at level $1-s$ before it. Between these two points, continuity and the first-passage choice give $1-s<F(x)<1$, with all intermediate levels attained. The interior $K_i$ of that segment therefore satisfies $F(K_i)=J$. The intervals $K_0,K_1$ are disjoint and lie inside $J$.

Thus [interval exactness produces a horseshoe](../../../../../../interval-exactness-produces-a-horseshoe.md):

$$
\boxed{T_s^N(K_0)=T_s^N(K_1)=J,\qquad K_0\cap K_1=\varnothing.}
$$

This is a [horseshoe for an interval map](../../../../../../horseshoe-for-an-interval-map.md) for an iterate of $T_s$, proving [Glendinning chaos](../../../../../../glendinning-chaos.md) for every $\sqrt2<s\leq2$. The proof does not require the same horseshoe iterate $N$ to work for every parameter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
