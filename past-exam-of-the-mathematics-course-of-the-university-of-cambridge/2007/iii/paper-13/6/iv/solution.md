<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Fix $p>1/2$, and use [separated-block percolation renormalization](../../../../../../separated-block-percolation-renormalization.md) to apply the preceding [one-independent bond percolation](../../../../../../one-independent-bond-percolation.md) result. Place a square

$$
S_v=3nv+[-n,n]^2
$$

at each coarse vertex $v\in\mathbb Z^2$. For a horizontal coarse edge $e=\{v,v+(1,0)\}$, let $R_e$ be the width-$5n$, height-$2n$ rectangle joining the two endpoint squares. Declare $e$ good if $R_e$ has a horizontal open crossing and both endpoint squares have vertical open crossings. For vertical coarse edges use the rotated definition.

The [rectangle crossing in bond percolation](../../../../../../rectangle-crossing-in-bond-percolation.md) limit proved above shows that each of these three events has probability tending to one. The [Harris lemma](../../../../../../harris-inequality.md) gives

$$
\mathbb P_p(e\text{ good})\geq h_p(5n,2n)h_p(2n,2n)^2\longrightarrow1.
$$

Choose $n$ so large that every coarse bond has good probability at least the $p_0<1$ from the preceding part.

The good-bond process really is one-independent. Its determining bonds lie entirely in the corresponding $R_e$. Nonincident horizontal coarse edges either lie in rows separated by at least $3n$, while their strips have width $2n$, or in the same row separated by at least one coarse edge; their rectangles are then separated by at least $n$. The vertical case is identical. A horizontal rectangle and a vertical rectangle can intersect only if the horizontal edge's endpoint column is the vertical edge's column and the vertical edge has an endpoint in the horizontal edge's row, which would make the coarse edges incident. Thus sets of nonincident coarse edges use disjoint fine-bond sets, and those sets are independent. The positive gap avoids the shared-boundary-bond problem that occurs with touching block constructions.

An infinite good coarse cluster produces an infinite connected fine open set. To verify connectivity, a long horizontal crossing of $R_e$ contains a horizontal crossing of each endpoint square. It therefore meets every vertical crossing of that square. For collinear good edges the transverse crossing of their shared square joins their long crossings; for perpendicular good edges their long crossings meet inside the shared square. Concatenating along the coarse cluster gives a connected open fine set visiting boxes at arbitrarily large distances.

The one-independent result gives positive probability that the coarse origin belongs to an infinite good cluster. On this event some vertex of the finite square $S_0$ belongs to an infinite fine open cluster. The [union bound](../../../../../../boole-s-inequality.md) and translation invariance of the original independent law imply

$$
0<\mathbb P_p(\exists x\in S_0:\ |C_x|=\infty)\leq|S_0|\theta(p),
$$

so $\theta(p)>0$. Since this holds for every $p>1/2$, and the [Harris theorem for square-lattice bond percolation](../../../../../../harris-theorem-for-square-lattice-bond-percolation.md) gives $\theta(p)=0$ for $p\leq1/2$, we obtain the [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md):

$$
\boxed{p_c(\mathbb Z^2)=1/2,\qquad\theta(1/2)=0,\qquad\theta(p)>0\text{ for every }p>1/2.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
