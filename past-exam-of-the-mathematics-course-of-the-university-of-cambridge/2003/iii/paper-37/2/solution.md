<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [linear polyhedron](../../../../../linear-polyhedron.md) $P\subseteq\mathbb R^n$ is full-dimensional if its [affine hull](../../../../../affine-hull.md) is $\mathbb R^n$. For a [convex set](../../../../../convex-set.md), this is equivalent to containing an open [Euclidean ball](../../../../../euclidean-ball.md): an open ball has full affine span, while $n+1$ [affinely independent](../../../../../affine-independence.md) points in the set span a [simplex](../../../../../simplex.md) with nonempty [interior](../../../../../interior-topology.md). In particular, a nonempty [linear polyhedron](../../../../../linear-polyhedron.md) need not be full-dimensional; a singleton or a [hyperplane](../../../../../hyperplane.md) is an example.

Assume $U\geq1$, increasing the coefficient bound to one if necessary. If $x_0\in P$ and $A_i$ denotes the $i$th row, then $\|A_i\|_2\leq\sqrt n U$. For $r=\varepsilon/(nU)$ and $\|h\|_2\leq r$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
A_i(x_0+h)\geq b_i-\|A_i\|_2\|h\|_2\geq b_i-\varepsilon.
$$

Thus **$B(x_0,r)\subseteq P_\varepsilon$ with $r>0$**, proving that $P_\varepsilon$ is a [full-dimensional linear polyhedron](../../../../../full-dimensional-linear-polyhedron.md). This part works for every positive $\varepsilon$; the particular small value also ensures that relaxation cannot create feasibility when $P$ is empty.

Here is that exact-feasibility point. Put $D=[(n+1)U]^{n+1}$. If $P$ is empty, a [Farkas certificate for linear inequalities](../../../../../farkas-certificate-for-linear-inequalities.md) gives $\lambda\geq0$ with $A^T\lambda=0$ and $b^T\lambda>0$. Normalize $\mathbf1^T\lambda=1$, and maximize $b^T\lambda$ over the compact [linear polyhedron](../../../../../linear-polyhedron.md)

$$
Q=\{\lambda\geq0:A^T\lambda=0,\ \mathbf1^T\lambda=1\}.
$$

Choose a maximizing [extreme point](../../../../../extreme-point.md). Its positive support has size $k\leq n+1$: a dependence among its supported columns $(A_i^T,1)$ would permit small perturbations of both signs in $Q$, contradicting extremality. Select $k$ independent equations for those $k$ coordinates. [Cramer's rule](../../../../../cramer-s-rule.md) expresses them over a common nonzero [integer](../../../../../integer.md) [determinant](../../../../../determinant.md) $\Delta$, with $|\Delta|\leq k!U^k\leq D$. Since $b$ is [integer](../../../../../integer.md) and $b^T\lambda>0$, its numerator is a positive [integer](../../../../../integer.md) after choosing a positive denominator. Hence $b^T\lambda\geq1/D$. This is the [normalized integer Farkas infeasibility gap](../../../../../normalized-integer-farkas-infeasibility-gap.md). A point in $P_\varepsilon$ would imply

$$
0=\lambda^TAx\geq b^T\lambda-\varepsilon\geq\frac1D-\frac1{2(n+1)D}>0,
$$

a contradiction. Consequently **$P=\varnothing$ if and only if $P_\varepsilon=\varnothing$**.

The [ellipsoid method](../../../../../ellipsoid-method.md) takes the [integer](../../../../../integer.md) [matrix](../../../../../matrix.md) $A$, [vector](../../../../../vector.md) $b$, dimension $n$, and a bound $U$ (or their binary encodings). It computes the prescribed $\varepsilon$, an inner radius $r$, and an outer radius $R$ whose logarithms have polynomial size. For an explicit outer bound, let $M=(nU)^n$. A nonempty $P$ has a [rational feasibility certificate for integer inequalities](../../../../../rational-feasibility-certificate-for-integer-inequalities.md) with $|x_j|\leq M$. To see this bound, intersect $P$ with an [orthant](../../../../../orthant.md) containing a feasible point. This intersection is a nonempty [linear polyhedron](../../../../../linear-polyhedron.md) containing no whole nontrivial affine line, and it has an [extreme point](../../../../../extreme-point.md). Indeed, if its active rows do not yet span the ambient space, move along a nonzero direction annihilating them. The [orthant](../../../../../orthant.md) prevents motion in both directions from being feasible forever, so in at least one direction a new independent row becomes active. Repeating at most $n$ times produces an [extreme point](../../../../../extreme-point.md). At that point choose $n$ independent [active constraints](../../../../../active-constraint.md), including coordinate constraints where needed. [Cramer's rule](../../../../../cramer-s-rule.md) and the [Hadamard determinant inequality](../../../../../hadamard-determinant-inequality.md) bound the numerators by $n^{n/2}U^n\leq M$, while a nonzero [integer](../../../../../integer.md) denominator has absolute value at least one. Thus the point has norm at most $nM$. Choosing $R=2nM+2$ ensures that, whenever $P$ is nonempty, an entire radius-$r$ [Euclidean ball](../../../../../euclidean-ball.md) in $P_\varepsilon$ lies inside $B(0,R)$.

Start with the [ellipsoid](../../../../../ellipsoid.md) $E_0=B(0,R)$ and retain $K=P_\varepsilon\cap B(0,R)$. At each iteration test the centre $c$ against every relaxed inequality. If it passes all tests, $P_\varepsilon$ is nonempty and hence so is $P$. Otherwise a violated row gives the [separation oracle](../../../../../separation-oracle.md): the feasible set lies in $\{x:A_i(x-c)\geq0\}$. Cut the current [ellipsoid](../../../../../ellipsoid.md) by this [half-space](../../../../../half-space.md) through its centre and replace it by the standard containing [ellipsoid](../../../../../ellipsoid.md). Every step retains $K$ and, for $n\geq2$, reduces [Lebesgue measure](../../../../../lebesgue-measure.md) by a factor at most $\exp[-1/(2(n+1))]$. In dimension one the corresponding step bisects an interval.

If more than $2n(n+1)\log(R/r)$ cuts occur without finding a feasible centre, the [Lebesgue measure](../../../../../lebesgue-measure.md) is smaller than that of a radius-$r$ ball. This contradicts the retained ball whenever $P$ is nonempty, so the [algorithm](../../../../../algorithm.md) can declare $P$ empty. Both $\log R$ and $\log(1/r)$ are polynomial in $n$ and $\log U$, and each inequality test uses $O(mn)$ arithmetic operations for $m$ rows. The bit implementation uses rational rounding with outward enlargement of the containing [ellipsoids](../../../../../ellipsoid.md); the encoding bounds allow polynomial precision while keeping a constant fraction of the volume decrease. Detailed update and rounding formulae are not needed for this account. The essential role of the [full-dimensional relaxation of integer inequalities](../../../../../full-dimensional-relaxation-of-integer-inequalities.md) is to supply a positive inner-volume bound without changing the emptiness decision; applying a [Lebesgue measure](../../../../../lebesgue-measure.md) stopping test directly to a lower-dimensional $P$ would fail.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
