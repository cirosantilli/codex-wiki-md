<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $H(R)$ and $V(R)$ for the horizontal and vertical open-crossing [increasing events](../../../../../../increasing-event.md) of a rectangle in the rotated [square lattice](../../../../../../square-lattice.md). At parameter $1/2$, [planar duality for rectangle crossings](../../../../../../planar-duality-for-rectangle-crossings.md) says that failure of $H$ is exactly a closed dual vertical crossing. Quarter-turn symmetry and the boundary convention of the rotated rectangles identify the two alternatives on a square. Thus its crossing [probability](../../../../../../probability.md) is $1/2$; a rectangle obtained by a harmless one-step boundary adjustment has crossing [probability](../../../../../../probability.md) at least $1/2$. This is the finite-domain [exact self-dual rectangle crossing probability](../../../../../../exact-self-dual-rectangle-crossing-probability.md), not an assumption about infinite [percolation clusters](../../../../../../percolation-cluster.md).

We first prove a [RSW reflection extension lemma](../../../../../../rsw-reflection-extension-lemma.md). In coordinate units adapted to the rotated drawing, take $S=[0,n]^2$, $T=[-n,n]^2$, and $R=[-n,2n]\times[-n,n]$. Reveal the rightmost open vertical crossing $\Gamma$ of $S$, when one exists, using only its [edges](../../../../../../edge-of-a-graph.md) and the region to its right. Reflect $\Gamma$ across the horizontal axis. The part $D$ of $T$ to the left of these two paths remains unexposed and has the independent parameter-$1/2$ law. A horizontal crossing of $T$ must reach their union. Its [probability](../../../../../../probability.md) is at least $1/2$. Reflection symmetry and the [union bound](../../../../../../boole-s-inequality.md) give a [probability](../../../../../../probability.md) at least $1/4$ of reaching the upper path $\Gamma$ through $D$. Conditional opening of the [edges](../../../../../../edge-of-a-graph.md) on $\Gamma$ can only help. Since $V(S)$ has [probability](../../../../../../probability.md) at least $1/2$, the [increasing event](../../../../../../increasing-event.md) $B$ that a vertical crossing of $S$ is connected inside $T$ to its left side has [probability](../../../../../../probability.md) at least $1/8$.

Reflect this construction in the vertical midline of $S$ to obtain an [increasing event](../../../../../../increasing-event.md) $B'$ of the same [probability](../../../../../../probability.md), connecting a vertical crossing of $S$ to the right side of $[0,2n]\times[-n,n]$. On $H(S)\cap B\cap B'$, the horizontal crossing of $S$ meets both vertical crossings, so all three [graph paths](../../../../../../path-in-a-graph.md) join and give $H(R)$. The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) now yields

$$
\mathbb P_{1/2}(H(R))\geq\frac12\left(\frac18\right)^2=\frac1{128}.
$$

The exploration only conditions the exposed side of the extremal [graph path](../../../../../../path-in-a-graph.md); reflecting a drawn path does not assert that its reflected [edges](../../../../../../edge-of-a-graph.md) are open. This distinction is what makes the extension argument valid.

To pass from aspect ratio $3/2$ to $3$, put four rectangles of width $3h/2$ and height $h$ next to each other, with successive left boundaries separated by $h/2$. Adjacent rectangles overlap in a square of side $h$. Require horizontal crossings of the four rectangles and vertical crossings of the three overlap squares. Every consecutive pair of horizontal crossings meets the vertical crossing in its overlap; together they form a horizontal crossing of width $3h$. The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) gives a strictly positive bound, for these compatible scales, of

$$
c_*=(1/128)^4(1/2)^3.
$$

The construction works on the rotated [square lattice](../../../../../../square-lattice.md) with the boundary sites used in the source drawing. Integer roundings do not create a scale restriction: for an odd height use the largest smaller compatible even height, and use eight horizontal rectangles and seven overlap squares, whose union has auxiliary aspect ratio $5$, so that its width exceeds the desired $3m$ width for all sufficiently large $m$. Truncate its horizontal crossing on first reaching the desired right side. The number of extra rectangles and overlap-square crossings is bounded independently of $m$, and every factor is bounded below by the same positive constants. The finitely many smallest rectangles each have positive crossing [probability](../../../../../../probability.md), since a specified finite open [graph path](../../../../../../path-in-a-graph.md) suffices. Therefore a constant $c>0$ works at every integer scale. Taking $\tau=c/2$ ensures the requested strict inequality:

$$
\boxed{\inf_{m\geq1}\mathbb P_{1/2}(C_{3m,m})\geq c>\tau>0}.
$$

This proves the required instance of the [Russo-Seymour-Welsh theorem](../../../../../../russo-seymour-welsh-theorem.md) through reflection, exploration and gluing. The parameter in this calculation is $1/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
