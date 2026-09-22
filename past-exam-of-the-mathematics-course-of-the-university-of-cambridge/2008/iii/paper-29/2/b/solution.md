<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A basis of open sets in the [p-adic integers](../../../../../../p-adic-integer.md) is

$$
\boxed{a+p^n\mathbb Z_p\qquad(a\in\mathbb Z_p,\ n\ge0).}
$$

Indeed this is the set of $x$ with $v_p(x-a)\ge n$, equivalently $|x-a|_p<p^{-(n-1)}$; these neighborhoods become arbitrarily small. Reduction identifies $\mathbb Z_p/p^n\mathbb Z_p$ with $\mathbb Z/p^n\mathbb Z$, so each has index $p^n$.

If a subgroup $H\le(\mathbb Z_p,+)$ is open, a neighborhood of zero of the displayed form lies inside $H$. Thus $p^n\mathbb Z_p\subseteq H$ for some $n$, and $[\mathbb Z_p:H]\le p^n$ is finite.

Conversely suppose the abstract index is the finite integer $m$. The quotient is a finite abelian group of order $m$, so Lagrange's theorem gives $mx\in H$ for every $x\in\mathbb Z_p$. Write $m=p^r u$ with $p\nmid u$. Multiplication by the [p-adic unit](../../../../../../p-adic-unit.md) $u$ is a bijection of $\mathbb Z_p$, its inverse being multiplication by $u^{-1}\in\mathbb Z_p$. Consequently

$$
p^r\mathbb Z_p=m\mathbb Z_p\subseteq H.
$$

The subgroup $H$ is a union of open cosets of $p^r\mathbb Z_p$, and is therefore open. This proves the characterization of [open subgroups of the p-adic integers](../../../../../../open-subgroups-of-the-p-adic-integers.md):

$$
\boxed{H\text{ open}\quad\Longleftrightarrow\quad[\mathbb Z_p:H]<\infty.}
$$

No prior assumption of closedness is required for the finite-index direction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
