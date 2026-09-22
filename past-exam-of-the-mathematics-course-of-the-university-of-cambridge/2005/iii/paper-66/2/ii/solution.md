<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The same relative coordinates give the [proximity time of translating line segments](../../../../../../proximity-time-of-translating-line-segments.md) as

$$
\boxed{\min t\quad\text{subject to}\quad\|D+sU-rT+tv\|\le d,\quad0\le s,r\le1,\quad t\ge0.}
$$

This is a convex norm-constrained problem, rather than the linear feasibility problem for contact. One can solve it as a small [second-order cone](../../../../../../second-order-cone.md) problem. If the distance between the initial [line segments](../../../../../../line-segment.md) is at most $d$, the answer is zero; if no [feasible point](../../../../../../feasible-point.md) exists, the threshold is never reached.

For an elementary analytic algorithm, consider the nine combinations in which each of $s,r$ is either free, fixed at zero or fixed at one. In each case, minimize the squared distance over the free parameters. Writing $q(t)$ for $D+tv$ plus the fixed endpoint contributions, and $K$ for the columns belonging to free parameters, stationarity is

$$
K^T(Kz+q(t))=0.
$$

If the [Gram matrix](../../../../../../gram-matrix.md) $K^TK$ is nonsingular, $z(t)=-(K^TK)^{-1}K^Tq(t)$ is affine in time. Retain only the time interval on which its entries lie in $[0,1]$. The residual is then $r_0+tr_1$, and feasibility reduces to

$$
\|r_1\|^2t^2+2(r_0\cdot r_1)t+\|r_0\|^2-d^2\le0.
$$

Intersect its solution interval with $t\ge0$ and the free-parameter validity interval, and record the first point. Include the four endpoint–endpoint cases, where there are no unfixed segment parameters. Take the earliest valid candidate among all cases. The actual closest pair belongs to one of these faces of the parameter square, so this enumeration cannot miss the first approach.

The complications are the quadratic threshold equation, changes of the active closest-point feature and singular [Gram matrices](../../../../../../gram-matrix.md) for parallel or degenerate segments. In a singular case, keep the affine family of minimizers and its feasibility bounds, or use the original convex problem; a pseudoinverse answer alone can fall outside the segment even when another minimizer is feasible. Constant-distance cases and tangential threshold contact must also be retained. Merely checking moving endpoints misses approaches between interior points.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
