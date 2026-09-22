<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $a<b$, give the pair $\{a,b\}$ the color determined by $v_2(b-a)\bmod2$, where $v_2$ is the [2-adic valuation](../../../../../2-adic-valuation.md): use red for even valuation and blue for odd valuation. This [finite coloring](../../../../../finite-coloring.md) works because the pairs $\{a,a+d\}$ and $\{a,a+2d\}$ have valuations $v_2(d)$ and $v_2(d)+1$. They therefore have opposite colors. In particular, **no three-term [arithmetic progression](../../../../../arithmetic-progression.md) has all its pairs [monochromatic](../../../../../monochromatic-set.md)**.

For the second assertion, $m=1$ is immediate: every singleton is a blue complete [arithmetic progression](../../../../../arithmetic-progression.md), since it has no pairs to check. Assume $m\geq2$. If some $m$-term [arithmetic progression](../../../../../arithmetic-progression.md) has all its pairs blue, we are done. Otherwise, every such [arithmetic progression](../../../../../arithmetic-progression.md) contains a red pair. For each $(a,d)\in\mathbb N^2$, choose, say lexicographically, indices $0\leq r<s<m$ for which $\{a+rd,a+sd\}$ is red, and color $(a,d)$ by this chosen pair $(r,s)$. This is a [finite coloring](../../../../../finite-coloring.md) with at most $\binom m2$ colors.

We need a lattice pattern that works whichever pair becomes the common color. Fix, before applying the [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md), the finite set

$$
F=\bigcup_{0\leq r<s<m}\{(si-rj,j-i):0\leq i,j<m\}\subseteq\mathbb Z^2.
$$

Translate $F$ into the positive quadrant and apply the [Gallai theorem for an integer lattice](../../../../../gallai-theorem-for-an-integer-lattice.md) to that translated pattern. Absorbing the translation into the base point gives integers $a_0,d_0$ and $q>0$ such that $(a_0,d_0)+qF\subseteq\mathbb N^2$ is [monochromatic](../../../../../monochromatic-set.md). Write $(r,s)$ for its common color. Since $(0,0)\in F$, the base point itself has positive coordinates.

For each $0\leq i,j<m$, the parameter point

$$
(a,d)=\bigl(a_0+q(si-rj),\ d_0+q(j-i)\bigr)
$$

belongs to that [monochromatic](../../../../../monochromatic-set.md) copy and has chosen red pair $(r,s)$. Its red endpoints simplify to

$$
a+rd=a_0+rd_0+q(s-r)i,\qquad a+sd=a_0+sd_0+q(s-r)j.
$$

Consequently, putting

$$
A=\{a_0+rd_0+q(s-r)i:0\leq i<m\},\qquad B=\{a_0+sd_0+q(s-r)j:0\leq j<m\},
$$

gives two $m$-term [arithmetic progressions](../../../../../arithmetic-progression.md) of positive [common difference](../../../../../common-difference.md) $q(s-r)$, with every cross-pair red. These [arithmetic progressions](../../../../../arithmetic-progression.md) really are disjoint: the parameter point corresponding to $i=m-1,j=0$ has positive second coordinate, so $d_0>q(m-1)$. Hence

$$
\min B-\max A=(s-r)\bigl(d_0-q(m-1)\bigr)>0.
$$

This proves the **[arithmetic-progression bipartite Ramsey dichotomy](../../../../../arithmetic-progression-bipartite-ramsey-dichotomy.md)**, including the required disjointness.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
