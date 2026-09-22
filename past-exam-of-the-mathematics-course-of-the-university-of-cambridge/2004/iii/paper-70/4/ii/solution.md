<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $N_{ij}(u,v)=B_i(u)C_j(v)$. Every available mixed [derivative](../../../../../../derivative.md) factors:

$$
\partial_u^a\partial_v^bN_{ij}=B_i^{(a)}(u)C_j^{(b)}(v).
$$

If the univariate factors have continuity $C^r$ and $C^s$, the right-hand side has equal one-sided traces across a $u$ knot for $a\leq r$, and across a $v$ knot for $b\leq s$. Their products therefore remain continuous, including where knot lines cross. The basis and its surface inherit coordinate-wise continuity orders $r,s$, and joint $C^{\min(r,s)}$ continuity. In particular, degree-$p$ and degree-$q$ [B-splines](../../../../../../b-spline.md) at simple knots give $C^{p-1}$ and $C^{q-1}$ continuity in the respective directions. Higher continuity can occur through special coefficient cancellation, but is not generally guaranteed.

Nonnegativity passes to products. Their [partition of unity](../../../../../../partition-of-unity.md) follows from

$$
\sum_{i,j}N_{ij}(u,v)=\left(\sum_iB_i(u)\right)\left(\sum_jC_j(v)\right)=1.
$$

Thus the surface remains in the [convex hull](../../../../../../convex-hull.md) of its active [control points](../../../../../../control-point.md) and commutes with application of [affine functions](../../../../../../affine-function.md). The support is the Cartesian product of the two univariate supports, giving local rectangular influence regions and efficient local evaluation. [Linear precision](../../../../../../linear-precision-of-a-geometric-basis.md) also passes independently in each coordinate. Clamped endpoint interpolation gives boundary curves determined by the outer rows/columns and corner interpolation; parameter-line curves inherit the corresponding univariate properties. These are the relevant inherited properties, rather than a claim of arbitrary global variation-diminishing behavior for surfaces.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
