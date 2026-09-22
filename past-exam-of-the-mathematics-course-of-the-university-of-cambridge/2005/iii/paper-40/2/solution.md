<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume $n\geq1$ and the [integer](../../../../../integer.md) coefficient bound $U\geq1$. There are $m(n+1)$ [integers](../../../../../integer.md) to record. Each signed [integer](../../../../../integer.md) in $[-U,U]$ can be encoded in $\lceil\log_2(2U+1)\rceil$ bits, so a fixed-width dense encoding needs

$$
m(n+1)\lceil\log_2(2U+1)\rceil+O(\log m+\log n+\log(U+1))
$$

bits, including the dimensions and bound. Its size is $\boxed{O(mn\log(U+1))}$. This is the bit-input model used for [polynomial time](../../../../../polynomial-time.md); an arithmetic-operation count alone would not suffice.

We first construct a [rational feasibility certificate for integer inequalities](../../../../../rational-feasibility-certificate-for-integer-inequalities.md). Choose a [feasible point](../../../../../feasible-point.md) and an [orthant](../../../../../orthant.md) containing it, adding coordinate inequalities of the form $x_i\geq0$ or $-x_i\geq0$. The intersection $Q$ is nonempty. Starting at a point of $Q$, if the [active constraint](../../../../../active-constraint.md) normals have rank less than $n$, choose a nonzero direction $d$ annihilating them. A sufficiently short move in either direction remains feasible, since every inactive constraint has positive slack. At least one direction has a finite endpoint: a nonzero coordinate of $d$ can be oriented toward the [orthant](../../../../../orthant.md) boundary. Move to the first constraint met along such a direction. Its normal does not annihilate $d$, so it is independent of the previously active normals. Their rank strictly increases. In at most $n$ moves we obtain a point with $n$ independent [active constraints](../../../../../active-constraint.md).

At that point $Bx=d_0$ for an invertible [integer](../../../../../integer.md) $n\times n$ [matrix](../../../../../matrix.md) $B$. Its rows are original constraint rows or signed coordinate rows, and $d_0$ has entries from $b$ or zero. All entries have absolute value at most $U$. By [Cramer's rule](../../../../../cramer-s-rule.md),

$$
x_i=\frac{\det B_i}{\det B},
$$

where $B_i$ replaces column $i$ by $d_0$. The [Hadamard determinant inequality](../../../../../hadamard-determinant-inequality.md) bounds both [determinants](../../../../../determinant.md) by $(\sqrt n\,U)^n\leq(nU)^n$. The denominator is a nonzero [integer](../../../../../integer.md). Hence each coordinate has the claimed representation with numerator and denominator bounded in absolute value by $R=(nU)^n$. The [orthant](../../../../../orthant.md) argument is needed because $P$ itself may contain lines and have no vertex. If $U=0$ is allowed literally, all coefficients and right sides vanish, and $x=0$ is feasible; the printed fraction bound then needs $U$ replaced by $\max(1,U)$, since a nonzero denominator cannot have absolute value at most zero. The bound just proved uses the customary positive coefficient bound.

Recording $n$ such fractions takes $O(n^2\log(nU))$ bits. A verifier checks that denominators are nonzero, changes their signs if needed, and verifies all inequalities by exact [integer](../../../../../integer.md) arithmetic after multiplying by positive denominators. The intermediate [integers](../../../../../integer.md) still have polynomial bit length. Thus a yes-instance has a polynomial-size, polynomial-time verifiable witness, and $\boxed{\mathrm{FP}\in\mathbf{NP}}$.

For optimization, let $c$ be rational with a finite binary encoding; clear its denominators to make it [integer](../../../../../integer.md), which multiplies the objective by a positive constant and preserves its minimizers. All bit bounds below include the encoding length of $c$. Let $V=\max(1,\max_i|c_i|)$ and $B_0=nVR$.

A useful refinement of the preceding vertex argument is that if an objective is bounded below, a [feasible point](../../../../../feasible-point.md) can be moved to an [orthant](../../../../../orthant.md) vertex without increasing its objective. Choose the annihilating direction to have $c^Td\leq0$. If the inequality is strict, the forward feasible interval must have a finite endpoint, since otherwise the objective would be unbounded below. If $c^Td=0$, choose either finite endpoint supplied by the [orthant](../../../../../orthant.md). Rank increases as before. There are only finitely many such vertices across the finitely many [orthants](../../../../../orthant.md). Every [feasible point](../../../../../feasible-point.md) therefore has one of these vertices with no larger objective; taking the least vertex value proves that a finite optimum is attained at one of them.

The Cramer representations at this optimum have one common denominator $\det B$, of magnitude at most $R$. Therefore its objective value $z^*$ has a representation with denominator at most $R$ and numerator at most $B_0$. In particular $|z^*|\leq B_0$. No enumeration of [orthants](../../../../../orthant.md) or vertices is part of the algorithm; they provide only polynomial-bit bounds.

Here is an [exact linear optimization from a feasibility oracle](../../../../../exact-linear-optimization-from-a-feasibility-oracle.md). First call the assumed [ellipsoid method](../../../../../ellipsoid-method.md) feasibility routine on $P$; if it is empty, report infeasibility. Otherwise query feasibility with the extra inequality $c^Tx\leq-B_0-1$. A yes answer proves unboundedness below, because any finite optimum would be at least $-B_0$; an unbounded objective necessarily gives a yes answer. Thus the infeasible, unbounded and finite-optimum cases are distinguished using two feasibility calls.

In the finite case, maintain an infeasible lower threshold $-B_0-1$ and a feasible upper threshold $B_0$. Bisect the interval, querying $c^Tx\leq t$ each time. After polynomially many calls its length is less than $1/(2R^2)$, and $z^*$ lies in the resulting interval. Distinct reduced fractions with positive denominators at most $R$ differ by at least $1/R^2$, so there is only one possible value. It can be recovered in [polynomial time](../../../../../polynomial-time.md) by [continued fractions](../../../../../continued-fraction.md): for the midpoint $t$, $|z^*-t|<1/(4R^2)\leq1/(2q^2)$, where $q\leq R$ is the denominator of $z^*$. Thus $z^*$ occurs among the continued-fraction convergents of $t$. Compute those by the Euclidean algorithm and choose the unique fraction with denominator at most $R$ in the interval. If $t=z^*$, use the final exact convergent. The Euclidean algorithm and all thresholds have polynomial bit length.

Even if the feasibility routine returns only a decision, an optimal point can be recovered without assuming a witness-producing oracle. Add $c^Tx=z^*$ and $-R\leq x_i\leq R$ for all $i$. This bounded optimal [convex polytope](../../../../../convex-polytope.md) is nonempty, since the optimal vertex above lies in it. Clear the denominator of $z^*$ and set

$$
H_0=\max\{1,U,R,B_0,VR\},\qquad D_0=(nH_0)^n.
$$

All vertex coordinates of this fixed [convex polytope](../../../../../convex-polytope.md) have denominators at most $D_0$ by the same [determinant](../../../../../determinant.md) argument. Minimize $x_1$, recover its exact minimum by feasibility bisection and rational reconstruction, then fix it; do the same for $x_2$, and so on. Each restriction is an [optimal face](../../../../../optimal-face-of-a-linear-program.md) of the same original bounded [convex polytope](../../../../../convex-polytope.md), so its vertices are original vertices. The single denominator bound $D_0$ therefore works at every step; repeated new precision bounds do not grow exponentially. After $n$ steps all coordinates are fixed to a feasible optimizer. There are polynomially many calls on polynomial-length rational instances, converted to [integer](../../../../../integer.md) inequalities by clearing denominators. Consequently **linear optimization has a polynomial-time algorithm whenever linear feasibility does**, with exact optimal value and optimizer, and correct reports of infeasibility or unboundedness.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
