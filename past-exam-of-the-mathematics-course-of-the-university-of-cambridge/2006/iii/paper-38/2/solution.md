<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In a [minimum-cost flow](../../../../../minimum-cost-flow-problem.md) problem, every directed arc $(i,j)$ has a per-unit cost $c_{ij}$ and lower and upper capacities $\ell_{ij},u_{ij}$. Each vertex has a prescribed net supply $b_i$, with $\sum_i b_i=0$. We seek flows minimizing $\sum_{ij}c_{ij}f_{ij}$ subject to the [flow conservation](../../../../../flow-conservation.md) equations

$$
\sum_jf_{ij}-\sum_jf_{ji}=b_i,\qquad
\ell_{ij}\leq f_{ij}\leq u_{ij}.
$$

The [uncapacitated minimum-cost flow](../../../../../uncapacitated-minimum-cost-flow.md) case has $u_{ij}=\infty$ and, here, $\ell_{ij}=0$.

For [project scheduling](../../../../../project-scheduling.md), augment the precedence graph with a source $0$, of duration $\tau_0=0$, and a sink $n+1$. Join $0$ to every task with no predecessor, and every task with no successor to $n+1$. Extend the precedence matrix to these dummy arcs. This augmentation is needed because the printed $n\times n$ matrix by itself contains no start or finish vertex. Assuming the precedence graph is a [Directed acyclic graph](../../../../../directed-acyclic-graph.md), every task lies on a source-to-sink path. Unlimited parallel work then gives the [linear programming](../../../../../linear-programming.md) formulation

$$
\boxed{\min(t_{n+1}-t_0),\qquad
t_j-t_i\geq\tau_i\quad\text{for every augmented arc }(i,j).}
$$

The time variables are unrestricted; a common translation changes nothing, so we may fix $t_0=0$. These inequalities say that each successor starts after its predecessor finishes. In a [topological order](../../../../../topological-order.md), their coordinatewise earliest solution is $t_j=\max_{i\to j}(t_i+\tau_i)$, the recursion of the [critical path method](../../../../../critical-path-method.md).

To derive [project scheduling duality](../../../../../project-scheduling-duality.md), associate a nonnegative multiplier $f_{ij}$ with $\tau_i+t_i-t_j\leq0$. The [Lagrangian](../../../../../lagrangian.md) is

$$
L(t,f)=t_{n+1}-t_0+\sum_{(i,j)}f_{ij}(\tau_i+t_i-t_j).
$$

Its infimum over the free time variables is finite precisely when the coefficients of all $t_i$ vanish. This gives one unit of net outflow at $0$, one unit of net inflow at $n+1$, and zero net [flow](../../../../../flow.md) at other vertices. Hence the dual is

$$
\max\sum_{(i,j)}\tau_i f_{ij}
\quad\text{subject to }f\geq0
\text{ and a unit flow from }0\text{ to }n+1.
$$

Equivalently, minimize $\sum c_{ij}f_{ij}$ with $c_{ij}=-\tau_i$. **The project duration is the negative of the optimal minimum-cost [flow](../../../../../flow.md) value.** The sign is essential: the dual of the minimization problem maximizes total duration, selecting a longest precedence path.

The [network simplex algorithm](../../../../../network-simplex-algorithm.md) is a general method for [minimum-cost flow](../../../../../minimum-cost-flow-problem.md). After shifting lower bounds to zero, first find a feasible [flow](../../../../../flow.md), using artificial arcs and a phase-one objective if needed. A [network simplex tree basis](../../../../../network-simplex-tree-basis.md) fixes each non-tree arc at a bound and determines the tree flows by [flow conservation](../../../../../flow-conservation.md). Choose [network dual potentials](../../../../../network-dual-potential.md) $\pi_i$ making the [network reduced cost](../../../../../network-reduced-cost.md)

$$
r_{ij}=c_{ij}-\pi_i+\pi_j
$$

zero on the tree. An arc at its [lower bound](../../../../../lower-bound-in-a-partially-ordered-set.md) is improving if $r_{ij}<0$; an arc at its [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) is improving in reverse if $r_{ij}>0$. Adding that residual arc creates one [fundamental cycle](../../../../../fundamental-cycle.md). Increase [flow](../../../../../flow.md) around this cycle until an arc reaches a bound, then exchange the entering and leaving tree arcs, or flip the entering arc to its other bound. The [flow conservation](../../../../../flow-conservation.md) equations remain satisfied. Use an anti-cycling rule for degenerate pivots. If a negative-cost residual cycle has no finite limiting capacity, the objective is unbounded below; if phase one cannot remove artificial [flow](../../../../../flow.md), the problem is infeasible. Otherwise, termination with no negative residual [network reduced costs](../../../../../network-reduced-cost.md) certifies optimality, since potentials cancel around cycles and every residual [network circulation](../../../../../circulation-in-a-flow-network.md) has nonnegative cost.

For this project the augmented arcs are

$$
(0,1),(0,2),(1,3),(2,4),(3,5),(4,5),(4,6),(5,7),(6,7).
$$

In the specified initial [spanning tree](../../../../../spanning-tree.md), the unique unit-flow path is $0\to1\to3\to5\to7$. The [flow](../../../../../flow.md) on its arcs is one and that on all other tree arcs is zero. Its total cost is $-3-5-4=-12$, so this is a degenerate but feasible [network simplex tree basis](../../../../../network-simplex-tree-basis.md). Normalizing $\pi_0=0$, the tree equations give

$$
(\pi_0,\ldots,\pi_7)=(0,0,-2,3,2,8,8,12).
$$

There are two nonbasic arcs. Their [network reduced costs](../../../../../network-reduced-cost.md) are

$$
r_{02}=0-\pi_0+\pi_2=-2,\qquad
r_{67}=-3-\pi_6+\pi_7=1.
$$

Bring $(0,2)$ into the tree. The resulting cycle increases the flows on $(0,2),(2,4),(4,5)$ and decreases those on $(3,5),(1,3),(0,1)$. The three decreasing arcs initially carry one unit, so the maximal step is one. Resolve the leaving-arc tie by removing $(0,1)$. The resulting unit [flow](../../../../../flow.md) follows $0\to2\to4\to5\to7$ and has cost $-4-6-4=-14$.

For the new tree, normalized potentials are

$$
(\pi_0,\ldots,\pi_7)=(0,2,0,5,4,10,10,14).
$$

The only nonbasic arcs now have $r_{01}=2$ and $r_{67}=1$, both nonnegative. All tree [network reduced costs](../../../../../network-reduced-cost.md) vanish, proving optimality after this single pivot. The earliest feasible schedule, obtained by the [critical path method](../../../../../critical-path-method.md), is

$$
\boxed{(t_0,t_1,t_2,t_3,t_4,t_5,t_6,t_7)
=(0,0,0,3,4,10,10,14),\qquad T^*=14.}
$$

The path $2\to4\to5$ has duration $4+6+4=14$, so it and the timetable furnish a [unit-flow certificate for project duration](../../../../../unit-flow-certificate-for-project-duration.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
