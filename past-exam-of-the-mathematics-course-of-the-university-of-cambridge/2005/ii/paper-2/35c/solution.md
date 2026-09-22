<h1 id="35c/solution">Solution</h1>

↑ **Parent:** [35C](../35c.md)

At a chosen event $p$, local inertial coordinates have $g_{ab}(p)=\eta_{ab}$, $\partial_cg_{ab}(p)=0$ and $\Gamma^a{}_{bc}(p)=0$. The metric agrees with Minkowski space to first order and freely falling trajectories are momentarily straight, expressing the local [Equivalence principle](../../../../../equivalence-principle.md). Second derivatives generally remain, recording [curvature](../../../../../curvature.md) and tidal effects.

Differentiate the [Levi-Civita connection](../../../../../levi-civita-connection.md). At $p$, the terms from derivatives of the inverse metric multiply first derivatives of $g$ and vanish, giving

$$
\partial_a\Gamma^c{}_{bd}
=\frac12\eta^{ce}(\partial_a\partial_bg_{ed}+\partial_a\partial_dg_{eb}-\partial_a\partial_eg_{bd}).
$$

For the convention $R^a{}_{bcd}=\partial_c\Gamma^a{}_{bd}-\partial_d\Gamma^a{}_{bc}+\Gamma\Gamma-\Gamma\Gamma$, the connection products vanish at $p$. Lowering the first index and subtracting these derivatives cancels the $\partial_c\partial_dg_{ab}$ terms, yielding

$$
\boxed{R_{abcd}=\frac12(\partial_b\partial_cg_{ad}+\partial_a\partial_dg_{bc}
-\partial_b\partial_dg_{ac}-\partial_a\partial_cg_{bd}).}
$$

Symmetry of $g$ and commutation of second derivatives show $R_{abcd}=R_{cdab}$ in these coordinates. Both sides are tensors, so equality in an inertial chart at each event implies equality at any point in every chart.

For the specified conformal metric, let $s=L^{-2}\eta_{ef}x^ex^f$. Its expansion is $g_{ab}=\eta_{ab}(1-2s+O(|x|^4))$. Thus the original coordinates are already inertial at zero, and

$$
\partial_c\partial_dg_{ab}(0)=-\frac4{L^2}\eta_{ab}\eta_{cd}.
$$

Substitution gives $R_{abcd}(0)=4(\eta_{ac}\eta_{bd}-\eta_{ad}\eta_{bc})/L^2$. In four dimensions the indicated contraction is

$$
\boxed{R(0)=\frac4{L^2}(4^2-4)=\frac{48}{L^2}.}
$$

The sign is fixed by the Riemann-tensor formula in the question; reversing the Riemann convention would reverse the scalar as well.

## ↑ Ancestors (10)

1. [35C](../35c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
