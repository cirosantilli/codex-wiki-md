<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use countably many copies of $A$, and let $c:S=\coprod_{i\geq1}A\to P=\prod_{i\geq1}A$ be the assumed isomorphism. Write $p_i=\pi_ic:S\to A$, let $\delta:A\to P$ be the diagonal with every component $1_A$, and put $q=c^{-1}\delta$. Thus $p_iq=1_A$ for every $i$. Let $s:S\to S$ shift the injections, $s\nu_i=\nu_{i+1}$, and let $\sigma:S\to A$ be the fold map, $\sigma\nu_i=1_A$.

The coordinate relations give $p_1s=0$ and $p_{i+1}s=p_i$, while $p_1\nu_1=1_A$ and $p_{i+1}\nu_1=0$. Therefore $q$ and $\nu_1+sq$ have identical $p_i$-coordinates. Since $c$ is invertible, these coordinates jointly distinguish arrows into $S$, so

$$
q=\nu_1+sq.
$$

The coproduct property gives $\sigma s=\sigma$, because both have value $1_A$ on each injection. Consequently $z=\sigma q$ satisfies

$$
z=\sigma\nu_1+\sigma sq=1_A+z.
$$

This proves the absorbing-endomorphism assertion without assuming an infinite addition operation on hom-sets.

If the category is an [additive category](../../../../../../additive-category.md), each hom-set is an [abelian group](../../../../../../abelian-group.md), so cancellation gives $1_A=0$. Any arrow $f:A\to B$ is then $f1_A=f0=0$. Every hom-set has exactly one arrow, and every object is isomorphic to the [zero object](../../../../../../zero-object.md). This is [countable biproducts in an additive category force triviality](../../../../../../countable-biproducts-in-an-additive-category-force-triviality.md):

$$
\boxed{z+1_A=z;\qquad\mathcal C\text{ additive}\ \Longrightarrow\ \mathcal C\simeq\mathbf1.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
