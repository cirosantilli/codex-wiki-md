<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Plünnecke's inequality](../../../../../../plunnecke-inequality.md) with the summand set also equal to $A$. There is a nonempty $X\subseteq A$ satisfying $|X+mA|\le C^m|X|$ for every $m\ge0$.

We need the [Ruzsa triangle inequality](../../../../../../ruzsa-triangle-inequality.md) in a form whose short proof also fixes the signs. For every $z\in R-S$, choose one representation $z=r_z-s_z$. The map

$$
(z,x)\longmapsto(r_z+x,s_z+x),\qquad x\in X,
$$

is injective into $(R+X)\times(S+X)$: its difference recovers $z$, then the fixed representation recovers $x$. Therefore

$$
|R-S||X|\le|R+X|\,|S+X|.
$$

Use $R=rA$ and $S=sA$ and the common set $X$ from the previous part:

$$
|rA-sA|\le\frac{|rA+X|\,|sA+X|}{|X|}
\le C^{r+s}|X|\le C^{r+s}|A|.
$$

Thus

$$
\boxed{|rA-sA|\le C^{r+s}|A|.}
$$

The shared minimizing subset is important; applying separate growth estimates with unrelated subsets would not justify this bound.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
