<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a [minimum-cost flow](../../../../../minimum-cost-flow-problem.md) problem, a [directed graph](../../../../../directed-graph.md) has arc flows $f_{ij}$, unit costs $c_{ij}$, lower and upper capacities $\ell_{ij},u_{ij}$, and net supplies $b_i$ summing to zero. The [linear program](../../../../../linear-programming.md) minimizes $\sum_{ij}c_{ij}f_{ij}$ subject to the [flow balances](../../../../../flow-balance.md) $\sum_j f_{ij}-\sum_j f_{ji}=b_i$ and $\ell_{ij}\leq f_{ij}\leq u_{ij}$.

Give each [graph vertex](../../../../../vertex-graph-theory.md) a [network dual potential](../../../../../network-dual-potential.md) $\pi_i$. With the outgoing-minus-incoming [oriented incidence matrix](../../../../../oriented-incidence-matrix.md) $B$, the [optimization Lagrangian](../../../../../optimization-lagrangian.md) is

$$
L(f,\pi)=c^Tf+\pi^T(b-Bf)
=\pi^Tb+\sum_{ij}r_{ij}f_{ij},\qquad
r_{ij}=c_{ij}-\pi_i+\pi_j.
$$

Minimizing over the capacity intervals is separable. A candidate [feasible flow](../../../../../feasible-flow.md) minimizes this [optimization Lagrangian](../../../../../optimization-lagrangian.md) if it takes its lower bound whenever the [network reduced cost](../../../../../network-reduced-cost.md) is positive, its upper bound whenever that [network reduced cost](../../../../../network-reduced-cost.md) is negative, and any allowed value when that [network reduced cost](../../../../../network-reduced-cost.md) is zero. Equivalently, for arcs with distinct lower and upper bounds,

$$
f_{ij}=\ell_{ij}\Rightarrow r_{ij}\geq0,\qquad
\ell_{ij}<f_{ij}<u_{ij}\Rightarrow r_{ij}=0,\qquad
f_{ij}=u_{ij}\Rightarrow r_{ij}\leq0.
$$

For every other [feasible flow](../../../../../feasible-flow.md) $g$, these conditions give $c^Tf=L(f,\pi)\leq L(g,\pi)=c^Tg$. This proves the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) certificate, rather than merely stating the [capacitated flow optimality conditions](../../../../../capacitated-flow-optimality-conditions.md).

Put $t=f_{23}$. The four [flow balances](../../../../../flow-balance.md) determine

$$
(f_{12},f_{23},f_{34},f_{41})=(t+3,t,t+1,t+2).
$$

Intersecting the four capacity intervals gives $2\leq t\leq4$. In particular,

$$
\boxed{f(2)=(5,2,3,4)}
$$

is a [feasible flow](../../../../../feasible-flow.md). Write $C=c_{12}+c_{23}+c_{34}+c_{41}$. Its cost along the feasible interval is

$$
c^Tf(t)=Ct+3c_{12}+c_{34}+2c_{41}.
$$

Hence $f(2)$ is optimal precisely when **$C\geq0$**. A [network dual potential](../../../../../network-dual-potential.md) certificate is

$$
\pi_1=0,\quad\pi_2=-c_{12},\quad
\pi_3=c_{41}+c_{34},\quad\pi_4=c_{41}.
$$

The three interior arcs have zero [network reduced costs](../../../../../network-reduced-cost.md) and $r_{23}=C$, which has the required nonnegative sign at its lower capacity.

For the [network simplex algorithm](../../../../../network-simplex-algorithm.md), start with the [network simplex tree basis](../../../../../network-simplex-tree-basis.md) consisting of arcs $12,34,41$, and fix nonbasic arc $23$ at its lower bound 2. These are exactly the potentials just found. If $C\geq0$, no improving pivot is needed. If $C<0$, arc $23$ enters and its fundamental [graph cycle](../../../../../cycle-in-a-graph.md) increases all four flows by the same amount. At $f(2)$ the remaining upper capacities are $(3,3,2,4)$, so the [simplex ratio test](../../../../../simplex-ratio-test.md) allows an increase of 2. Arc $34$ reaches its upper bound and leaves the tree. The new [network simplex tree basis](../../../../../network-simplex-tree-basis.md) has arcs $12,23,41$, with potentials

$$
\pi_1=0,\quad\pi_2=-c_{12},\quad
\pi_3=-c_{12}-c_{23},\quad\pi_4=c_{41}.
$$

Now only the nonbasic arc $34$ has a possibly nonzero [network reduced cost](../../../../../network-reduced-cost.md), namely $r_{34}=C<0$. It is at its upper bound, so the sign is optimal. Thus for all real costs the complete answer is

$$
\boxed{\begin{cases}
f(2)=(5,2,3,4),&C>0,\\
f(t),\quad2\leq t\leq4,&C=0,\\
f(4)=(7,4,5,6),&C<0.
\end{cases}}
$$

When $C=0$, both endpoint [basic feasible solutions](../../../../../basic-feasible-solution.md) and every intermediate [feasible flow](../../../../../feasible-flow.md) have the same cost.

To count [basic solutions](../../../../../basic-solution.md), a [network simplex tree basis](../../../../../network-simplex-tree-basis.md) omits one arc of the four-cycle and fixes that arc at either bound. The possibilities are

$$
\begin{array}{c|c|c|c}
\text{nonbasic arc}&\text{bound used}&t&\text{feasible?}\\\hline
12&\text{lower}&0&\text{no}\\
12&\text{upper}&5&\text{no}\\
23&\text{lower}&2&\text{yes}\\
23&\text{upper}&5&\text{no}\\
34&\text{lower}&1&\text{no}\\
34&\text{upper}&4&\text{yes}\\
41&\text{lower}&-2&\text{no}\\
41&\text{upper}&6&\text{no}
\end{array}
$$

There are **eight tree/bound basic representations, seven distinct basic flow vectors, and two basic feasible solutions**. The distinction in the first count matters: the upper bounds on $12$ and $23$ both give the identical flow $(8,5,6,7)$ at $t=5$. Thus if “basic solutions” counts vectors rather than basis representations, the answer to (i) is seven; the frequently used count of basis/bound choices is eight. The answer to (ii) is unambiguously two, since only $t=2,4$ satisfy all capacities.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
