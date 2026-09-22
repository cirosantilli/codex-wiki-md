<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [prime ideal](../../../../../../prime-ideal.md) $P$ is a proper [ideal](../../../../../../ideal.md) such that $ab\in P$ implies $a\in P$ or $b\in P$. Equivalently $R/P$ is an [integral domain](../../../../../../integral-domain.md).

For each $i$, and each $j\ne i$, choose $a_{ji}\in P_j\setminus P_i$, using incomparability. Put

$$
b_i=\prod_{j\ne i}a_{ji}.
$$

Then $b_i$ belongs to the other two [prime ideals](../../../../../../prime-ideal.md) and does not belong to $P_i$, by primality. In particular each $b_i$ lies in the union. But $b_1+b_2+b_3\notin P_i$ for every $i$: modulo $P_i$, the sum equals $b_i\ne0$. **The union is not closed under addition and is not an [ideal](../../../../../../ideal.md).** This is a concrete instance of [prime avoidance](../../../../../../prime-avoidance.md).

The [union of three incomparable nonprime ideals](../../../../../../union-of-three-incomparable-nonprime-ideals.md) example can retain pairwise incomparability. In the [ring](../../../../../../ring.md)

$$
R=\mathbb F_2[u,v]/(u^2,uv,v^2),
$$

take

$$
\boxed{I_1=(u),\qquad I_2=(v),\qquad I_3=(u+v).}
$$

These distinct two-element [ideals](../../../../../../ideal.md) are pairwise incomparable, yet

$$
I_1\cup I_2\cup I_3=\{0,u,v,u+v\}=(u,v),
$$

which is an [ideal](../../../../../../ideal.md). None is prime: its [quotient ring](../../../../../../quotient-ring.md) still contains a nonzero element of square zero. The three one-dimensional [vector subspaces](../../../../../../vector-subspace.md) cover the two-dimensional [vector space](../../../../../../vector-space-split.md) over $\mathbb F_2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
