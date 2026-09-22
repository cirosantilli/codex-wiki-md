<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [Gallai theorem for an integer lattice](../../../../../../gallai-theorem-for-an-integer-lattice.md) to the finite pattern

$$
F=\bigcup_{0\le r<s<m}\{(su-rv,\ v-u):0\le u,v<m\}\subseteq\mathbb Z^2.
$$

Although some coordinates are negative, translating $F$ into the positive quadrant and applying the positive-lattice theorem produces a [monochromatic](../../../../../../monochromatic-set.md) copy $F_0=(a_0,d_0)+qF\subseteq\mathbb N^2$, with integer $q>0$. The translation is absorbed into $(a_0,d_0)$. Let $(r,s)$ be the common position-pair label on this copy.

For each $0\le u,v<m$, the starting point and step

$$
a=a_0+q(su-rv),\qquad d=d_0+q(v-u)
$$

label the red edge at positions $r,s$. Its endpoints simplify to

$$
a+rd=a_0+rd_0+q(s-r)u,\qquad
a+sd=a_0+sd_0+q(s-r)v.
$$

Thus the two [arithmetic progressions](../../../../../../arithmetic-progression.md)

$$
A=\{a_0+rd_0+q(s-r)u:0\le u<m\},\qquad
B=\{a_0+sd_0+q(s-r)v:0\le v<m\}
$$

have a positive [common difference](../../../../../../common-difference.md) $q(s-r)$, and every cross-pair is red. Their entries are positive because they occur as endpoints of the positive-start, positive-step progressions represented in $F_0$.

It remains to check disjointness, rather than infer it merely from distinct starting points. The pattern contains points whose second coordinate is $-(m-1)$. Since all of $F_0$ lies in $\mathbb N^2$,

$$
d_0-q(m-1)>0.
$$

Consequently

$$
\min B-\max A=(s-r)\bigl[d_0-q(m-1)\bigr]>0.
$$

Therefore **$A$ and $B$ are disjoint $m$-term [arithmetic progressions](../../../../../../arithmetic-progression.md) with every cross-edge red**. Combined with the first branch, this proves the dichotomy.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
