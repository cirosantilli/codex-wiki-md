<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret $Y_n$ as the length of a shortest [Euclidean travelling salesman tour](../../../../../../euclidean-travelling-salesman-tour.md), and take the points to be [independent random variables](../../../../../../independent-random-variables.md) with the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on the square. We assume $n\geq2$; a closed tour on one point has length zero, so the printed lower bound would be false for $n=1$. For two points the closed tour traverses the joining segment twice.

For the deterministic upper bound, use the following precise geometric result, the [squared edge bound for tours in the unit square](../../../../../../squared-edge-bound-for-tours-in-the-unit-square.md): every finite set of points in $[0,1]^2$ admits a cyclic ordering $z_1,\ldots,z_n$ such that

$$
\sum_{i=1}^n\lVert z_{i+1}-z_i\rVert^2\leq4,\qquad z_{n+1}=z_1.
$$

Here is a proof of that geometric result. First consider a [right triangle](../../../../../../right-triangle.md) with hypotenuse endpoints $a,b$, hypotenuse length $c$, and right-angle vertex $v$. The [quadratic path bound in a right triangle](../../../../../../quadratic-path-bound-in-a-right-triangle.md) supplies a path from $a$ to $b$ through any finite set inside the triangle whose sum of squared edge lengths is at most $c^2$. For an empty set use the edge $ab$. For a single point $z$, use $a,z,b$: the triangle lies in the disk with diameter $ab$, so $\angle azb\geq\pi/2$ and the [law of cosines](../../../../../../law-of-cosines.md) gives $\lVert a-z\rVert^2+\lVert z-b\rVert^2\leq c^2$.

For several points, draw the [altitude](../../../../../../altitude.md) from $v$ to the hypotenuse. It splits the triangle into two smaller [right triangles](../../../../../../right-triangle.md) with hypotenuses $av$ and $vb$. Their squared hypotenuse lengths sum to $c^2$ by the [Pythagorean theorem](../../../../../../pythagorean-theorem.md). Repeated [altitude](../../../../../../altitude.md) subdivision eventually makes every cell small enough to contain at most one of the given distinct points: each child is similar to the original triangle and its diameter contracts by at most the fixed factor $\max(\lVert a-v\rVert,\lVert b-v\rVert)/c<1$. Construct the base-case paths and combine them from the bottom of this finite subdivision tree. The two child paths concatenate at $v$. If $v$ is an auxiliary point, delete it by joining its two neighbours directly. Both neighbours lie in the right-angle sector of the parent triangle at $v$, so their angle at $v$ is at most $\pi/2$. The [law of cosines](../../../../../../law-of-cosines.md) now shows that this shortcut does not increase the sum of squared edge lengths. The combined path still has endpoints $a,b$ and squared cost at most $c^2$.

One can first put the given points in generic positions, avoiding subdivision boundaries, and then pass to a limit. There are only finitely many possible visiting orders, so a subsequence keeps the same order and its squared cost converges; this also handles coincident locations. No assumption about a minimum separation remains in the result.

Split the square along a diagonal $ab$. Apply the triangle result in each half, following one path from $a$ to $b$ and the other back to $a$. Each half contributes at most $\lVert a-b\rVert^2=2$. Remove either diagonal endpoint if it was auxiliary. At a square corner all neighbours lie in a sector of angle $\pi/2$, so the same squared-cost shortcut applies. This gives the asserted cyclic ordering with total squared cost at most four. It does not assert that the tour minimizing ordinary length itself has this squared-edge property. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) applied to the tour supplied by the theorem proves

$$
Y_n\leq\sum_i\lVert z_{i+1}-z_i\rVert\leq\sqrt{n\sum_i\lVert z_{i+1}-z_i\rVert^2}\leq2\sqrt n.
$$

Thus **the upper bound is deterministic**, independently of the sampling law.

For the lower bound, put $R_i=\min_{j\ne i}\lVert X_i-X_j\rVert$, the [nearest neighbour distance](../../../../../../nearest-neighbour-distance.md) at $X_i$. Both edges incident to $X_i$ in any closed tour have length at least $R_i$. Summing over vertices and then dividing by two gives $Y_n\geq\sum_iR_i$. Conditional on $X_i=x$, the [union bound](../../../../../../boole-s-inequality.md) and the [uniform distribution](../../../../../../continuous-uniform-distribution.md) give

$$
\mathbb P(R_i<t\mid X_i=x)\leq(n-1)\lambda_2(B(x,t)\cap[0,1]^2)\leq(n-1)\pi t^2.
$$

Boundary clipping only makes the ball smaller. Apply the [layer cake representation](../../../../../../layer-cake-representation.md) of the [expected value](../../../../../../expected-value.md), restricting the integral to $0\leq t\leq1/(2\sqrt n)$:

$$
\begin{aligned}
\mathbb ER_i&=\int_0^\infty\mathbb P(R_i\geq t)\,dt\\
&\geq\int_0^{1/(2\sqrt n)}(1-(n-1)\pi t^2)\,dt\\
&=\frac1{2\sqrt n}-\frac{(n-1)\pi}{24n^{3/2}}\geq\frac{1/2-\pi/24}{\sqrt n}>\frac1{5\sqrt n}.
\end{aligned}
$$

Linearity of the [expected value](../../../../../../expected-value.md) now yields

$$
\boxed{Y_n\leq2\sqrt n,\qquad\mathbb EY_n\geq\frac{\sqrt n}{5}.}
$$

The unspecified sampling phrase in the paper must therefore be understood as independent uniform sampling: an arbitrary distribution concentrated in a tiny region cannot satisfy this lower bound.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
