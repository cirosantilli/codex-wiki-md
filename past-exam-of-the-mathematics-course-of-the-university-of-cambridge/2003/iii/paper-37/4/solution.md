<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Nash bargaining problem](../../../../../nash-bargaining-problem.md) consists of a [compact convex set](../../../../../compact-convex-set.md) $S$ of feasible two-player [payoff](../../../../../payoff.md) [vectors](../../../../../vector.md) and a [disagreement point](../../../../../disagreement-point.md) $d\in S$. If bargaining fails, the players receive $d$; agreement selects a feasible [vector](../../../../../vector.md). The [convex set](../../../../../convex-set.md) allows jointly agreed [correlated payoff lotteries](../../../../../lottery-over-joint-action-profiles.md) over outcomes. Assume essentiality: some feasible [vector](../../../../../vector.md) strictly improves both coordinates of $d$. The admissible answers satisfy [bargaining individual rationality](../../../../../bargaining-individual-rationality.md), $u_i\geq d_i$.

The four characterizing axioms are [Pareto efficiency](../../../../../pareto-efficiency.md) (no feasible [vector](../../../../../vector.md) weakly improves both chosen [payoffs](../../../../../payoff.md) and strictly improves one), [bargaining symmetry](../../../../../bargaining-symmetry.md) (interchanging identical player roles leaves the answer unchanged), [positive affine invariance in bargaining](../../../../../positive-affine-invariance-in-bargaining.md) (independently replacing utilities by $a_i u_i+b_i$, $a_i>0$, transforms the answer by the same maps), and [bargaining independence of irrelevant alternatives](../../../../../bargaining-independence-of-irrelevant-alternatives.md) (restricting to an admissible smaller feasible set that still contains the chosen [vector](../../../../../vector.md) leaves the choice unchanged). The last axiom keeps the [disagreement point](../../../../../disagreement-point.md) fixed.

The arbitration procedure maximizes the [Nash product](../../../../../nash-product.md) over individually rational [vectors](../../../../../vector.md):

$$
f(S,d)=\operatorname*{argmax}_{u\in S,\ u\geq d}(u_1-d_1)(u_2-d_2).
$$

A maximizer exists by [compactness](../../../../../compact-space.md) and has positive gains by essentiality. It is unique, since the [logarithm](../../../../../logarithm.md) of the product is a [strictly concave function](../../../../../strictly-concave-function.md) of the two gains on their positive domain. The product is strictly increasing in either positive gain, giving [Pareto efficiency](../../../../../pareto-efficiency.md). A positive affine utility change multiplies the product by $a_1a_2$, giving [positive affine invariance in bargaining](../../../../../positive-affine-invariance-in-bargaining.md). Uniqueness gives [bargaining symmetry](../../../../../bargaining-symmetry.md) and [bargaining independence of irrelevant alternatives](../../../../../bargaining-independence-of-irrelevant-alternatives.md).

For completeness, these axioms also force the procedure. Normalize the product-maximizing [vector](../../../../../vector.md) to $(1,1)$ and $d$ to zero using [positive affine invariance in bargaining](../../../../../positive-affine-invariance-in-bargaining.md). For any normalized feasible [vector](../../../../../vector.md) $z$, the [directional derivative](../../../../../directional-derivative.md) of the product along the feasible segment from $(1,1)$ to $z$ is $z_1+z_2-2$. The initial part of that segment has positive gains, so optimality implies $z_1+z_2\leq2$. Choose $M$ sufficiently large that the transformed feasible set is contained in the symmetric triangle

$$
T_M=\{z:z_1,z_2\geq-M,\ z_1+z_2\leq2\}.
$$

On this triangle, [bargaining symmetry](../../../../../bargaining-symmetry.md) requires equal coordinates and [Pareto efficiency](../../../../../pareto-efficiency.md) then forces $(1,1)$. By [bargaining independence of irrelevant alternatives](../../../../../bargaining-independence-of-irrelevant-alternatives.md), restricting from $T_M$ to the original normalized set still selects $(1,1)$. Undoing the normalization proves the [Nash bargaining solution](../../../../../nash-bargaining-solution.md) characterization. This is the [supporting triangle for Nash bargaining](../../../../../supporting-triangle-for-nash-bargaining.md) argument.

For the numerical game, the maximin [disagreement point](../../../../../disagreement-point.md) is the [vector](../../../../../vector.md) of the players' separate [security level payoffs](../../../../../security-level-payoff.md). If player I uses its first action with [probability](../../../../../probability.md) $p$, its worst expected [payoff](../../../../../payoff.md) is

$$
\min\{4-2p,\ 2+6p\}.
$$

The two lines meet at $p=1/4$; before that point the increasing second line is smaller and afterwards the decreasing first line is smaller. Hence $d_1=7/2$. If player II uses its first action with [probability](../../../../../probability.md) $q$, its worst [payoff](../../../../../payoff.md) is

$$
\min\{2+2q,\ 3+2q\}=2+2q,
$$

maximized at $q=1$, giving $d_2=4$. Thus **$d=(7/2,4)$**. These are separate worst-case guarantees; they need not equal the actual [payoffs](../../../../../payoff.md) when both security strategies are used together.

The cooperative feasible set is the [convex hull](../../../../../convex-hull.md) of the four outcome [vectors](../../../../../vector.md). The outcomes $(2,4)$ and $(2,3)$ are dominated by $C=(4,5)$. Its [Pareto frontier](../../../../../pareto-frontier.md) is the segment joining $C$ to $B=(8,2)$, with equation $y=8-3x/4$. Any maximizer of the positive [Nash product](../../../../../nash-product.md) is on this frontier. [Bargaining individual rationality](../../../../../bargaining-individual-rationality.md) restricts its relevant portion to $4\leq x\leq16/3$. There we maximize

$$
g(x)=(x-7/2)(4-3x/4),\qquad g'(x)=\frac{53}{8}-\frac32x,\qquad g''(x)=-\frac32.
$$

The stationary point lies strictly inside that interval and is the unique maximum. Therefore **the [Nash bargaining solution](../../../../../nash-bargaining-solution.md) is**

$$
\boxed{(x,y)=\left(\frac{53}{12},\frac{75}{16}\right).}
$$

The gains are $11/12$ and $11/16$, with [Nash product](../../../../../nash-product.md) $121/192$. The arbitration can implement the [vector](../../../../../vector.md) by the agreed [correlated payoff lottery](../../../../../lottery-over-joint-action-profiles.md) assigning [probability](../../../../../probability.md) $5/48$ to outcome $B$ and $43/48$ to outcome $C$. Indeed $4+4(5/48)=53/12$ and $5-3(5/48)=75/16$. This is a [correlated payoff lottery](../../../../../lottery-over-joint-action-profiles.md); independent [mixed strategies](../../../../../mixed-strategy.md) are not required to implement the cooperative agreement.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
