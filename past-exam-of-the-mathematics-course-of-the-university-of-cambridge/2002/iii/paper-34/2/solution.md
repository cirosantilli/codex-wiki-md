<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $x$ be an [extreme point](../../../../../extreme-point.md) and consider its [active constraints](../../../../../active-constraint.md). Their row vectors span $\mathbb R^n$. Otherwise a nonzero vector $h$ is orthogonal to every active row. All inactive inequalities have strictly positive slack; since there are finitely many, a sufficiently small $\varepsilon>0$ makes both $x+\varepsilon h$ and $x-\varepsilon h$ feasible. Their midpoint is $x$, contradicting extremality.

Choose $n$ independent active rows and write the corresponding equalities as $Bx=d$. The [matrix](../../../../../matrix.md) $B$ has [integer](../../../../../integer.md) entries, so $\det B$ is a nonzero [integer](../../../../../integer.md) and $|\det B|\ge1$. By [Cramer's rule](../../../../../cramer-s-rule.md),

$$
x_j=\frac{\det B_j}{\det B},
$$

where $B_j$ replaces column $j$ by $d$. Every entry of $B_j$ has absolute value at most $U$, even when $b$ is real. The [determinant](../../../../../determinant.md) expansion has $n!$ terms, each with absolute value at most $U^n$. Therefore

$$
\boxed{|x_j|\le n!U^n\quad(1\le j\le n).}
$$

This proves the [integer-matrix vertex coordinate bound](../../../../../integer-matrix-vertex-coordinate-bound.md); only the denominator [determinant](../../../../../determinant.md) requires integrality.

For an exact finite-input [ellipsoid method](../../../../../ellipsoid-method.md), the numerical data must have a specified encoding. In the standard model the input is the dimensions, the [integer](../../../../../integer.md) [matrix](../../../../../matrix.md) and a rational right-hand side in binary, together with bounds derived from their encoding lengths. The vertex estimate above remains valid for arbitrary real $b$, but arbitrary unencoded reals do not by themselves specify an exact computational decision problem. Clear the rational row denominators to obtain an equivalent [integer](../../../../../integer.md) system, and let $V\ge1$ bound the resulting [integer](../../../../../integer.md) coefficients and right-hand sides.

Two precautions make a feasibility account valid even for unbounded or lower-dimensional polyhedra. First, nonempty polyhedra need not have [extreme points](../../../../../extreme-point.md). Nevertheless they have a [feasible point](../../../../../feasible-point.md) in the box $[-R,R]^n$ with $R=n!V^n$. To prove this [feasible-point box bound for a polyhedron with lines](../../../../../feasible-point-box-bound-for-a-polyhedron-with-lines.md), intersect the polyhedron with an orthant containing one [feasible point](../../../../../feasible-point.md). Minimize the sum of the signed coordinates in that orthant. Its nonempty sublevel sets are closed and bounded, so the minimum is attained. The compact minimum face has an [extreme point](../../../../../extreme-point.md), which is also extreme in the orthant intersection. Its active rows come from the [integer](../../../../../integer.md) system and signed coordinate inequalities, still bounded by $V$. Applying the proved vertex estimate gives the box bound. This is an existence argument; the algorithm need not enumerate all orthants.

Second, a nonempty feasible set can have zero ambient volume. Use a small uniform relaxation with a certified rational infeasibility gap, rather than stopping on volume alone. For the [integer](../../../../../integer.md) system $\widetilde A x\ge\widetilde b$, put

$$
D=[(n+1)V]^{n+1},\qquad \eta=\frac1{2D}.
$$

The [normalized integer Farkas infeasibility gap](../../../../../normalized-integer-farkas-infeasibility-gap.md) says that if the system is empty there is a multiplier $y\ge0$ with $\widetilde A^Ty=0$, $\mathbf1^Ty=1$ and $\widetilde b^Ty\ge1/D$. Its bound follows by maximizing the certificate's value in the normalized multiplier polytope: a vertex has at most $n+1$ positive entries, and a [determinant](../../../../../determinant.md) denominator bounded by $D$. Any point satisfying the relaxed inequalities would then give the contradiction

$$
0=y^T\widetilde A x\ge y^T\widetilde b-\eta\ge\frac1{2D}>0.
$$

Thus relaxation preserves emptiness. If the original system is nonempty, take its point $x_0\in[-R,R]^n$. The bounded relaxed set

$$
Q=\{x:\widetilde A x\ge\widetilde b-\eta\mathbf1,\quad |x_j|\le R+1\}
$$

contains a Euclidean ball around $x_0$ of radius $\rho=\min(1/2,\eta/(nV))$: each row changes by at most $\sqrt nV\rho\le\eta$, and the expanded box leaves room for the ball. Hence $Q$ is either empty or has an explicit positive inner-volume bound. This is the [full-dimensional relaxation of integer inequalities](../../../../../full-dimensional-relaxation-of-integer-inequalities.md) principle.

Start with a ball, viewed as an [ellipsoid](../../../../../ellipsoid.md), centered at zero with radius $n(R+1)$, which contains the search box. At each iteration test its center against all inequalities defining $Q$. If the center is feasible, the preserved-emptiness result answers that the original problem is nonempty. Otherwise a violated row supplies a [separation oracle](../../../../../separation-oracle.md) cut. Move that cut parallel to itself through the current center if necessary, and compute a smaller containing [ellipsoid](../../../../../ellipsoid.md) for the surviving half. Every [feasible point](../../../../../feasible-point.md) remains in the new [ellipsoid](../../../../../ellipsoid.md).

The [central-cut ellipsoid volume bound](../../../../../central-cut-ellipsoid-volume-bound.md) gives a shrinkage factor at most $e^{-1/(2(n+1))}$ for $n\ge2$. After $O(n^2\log(n(R+1)/\rho))$ cuts, the volume is below that of a radius-$\rho$ ball. If no feasible center has been found, $Q$ and therefore the original system are empty. Dimension one uses interval bisection. The logarithms of $R$, $D$ and $1/\rho$ are polynomial in the encoded input size. Standard outward-controlled finite-precision [ellipsoid](../../../../../ellipsoid.md) updates preserve enclosure with polynomial bit complexity.

The coordinate bound therefore supplies the initial bounded search region; the rational gap supplies a valid stopping threshold. Neither unboundedness nor zero volume of the original polyhedron can be ignored when deciding emptiness.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
