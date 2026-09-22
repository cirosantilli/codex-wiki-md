<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $(j_1,\ldots,j_k)$ for the partial [assignment problem](../../../../../assignment-problem.md) solution sending person $i$ to job $j_i$. The prescribed [assignment lower bound from independent task minima](../../../../../assignment-lower-bound-from-independent-task-minima.md) is

$$
L(j_1,\ldots,j_k)=\sum_{i=1}^k a_{i,j_i}+\sum_{j\notin\{j_1,\ldots,j_k\}}\min_{i>k}a_{ij}.
$$

Every completion must pay at least the minimum in each remaining column, so this is a valid [lower bound](../../../../../lower-bound-in-a-partially-ordered-set.md), even if the minima use the same person several times. At $k=3$, the one remaining job must go to person 4, and the bound is the exact completed cost.

Use [branch and bound](../../../../../branch-and-bound.md) with the smallest open bound expanded first. The initial bounds are

$$
\begin{array}{c|rrrr}
\text{prefix}&(1)&(2)&(3)&(4)\\
L&60&58&65&78
\end{array}
$$

For example, $L(2)=12+11+13+22=58$. Expand $(2)$, giving

$$
L(2,1)=68,\qquad L(2,3)=59,\qquad L(2,4)=64.
$$

Expand $(2,3)$. Its children are $(2,3,1)$ with bound 64 and $(2,3,4)$ with bound 65. Completing the first gives $(2,3,1,4)$ at cost 64, our first incumbent. The second cannot improve it. We may also discard $(2,1)$, $(2,4)$, $(3)$ and $(4)$, since their [lower bounds](../../../../../lower-bound-in-a-partially-ordered-set.md) are at least 64; equality may be pruned when seeking one optimum.

The remaining open prefix is $(1)$, whose children have bounds

$$
L(1,2)=68,\qquad L(1,3)=61,\qquad L(1,4)=66.
$$

Only $(1,3)$ can improve the incumbent. Its children $(1,3,2)$ and $(1,3,4)$ have exact completed costs 69 and 61, respectively. The latter completes to $(1,3,4,2)$ and replaces the incumbent. Every other branch has already been bounded above this value. Thus **the optimal assignment is**

$$
\boxed{1\mapsto1,\quad2\mapsto3,\quad3\mapsto4,\quad4\mapsto2,\qquad \text{cost}=11+13+23+14=61.}
$$

This [branch and bound](../../../../../branch-and-bound.md) computation produces fourteen partial nodes: four initial nodes, three below $(2)$, two below $(2,3)$, three below $(1)$ and two below $(1,3)$. The last person is assigned automatically at a depth-three node.

For the [travelling salesman problem](../../../../../travelling-salesman-problem.md), let $x_{ij}=1$ mean that the tour goes directly from city $i$ to city $j$. Retain only the constraints

$$
\sum_{j\ne i}x_{ij}=1,\qquad \sum_{i\ne j}x_{ij}=1,\qquad x_{ij}\in\{0,1\},\quad x_{ii}=0.
$$

This is an [assignment problem](../../../../../assignment-problem.md) between cities as departure points and cities as arrival points, solvable by the [Hungarian algorithm](../../../../../hungarian-algorithm.md). Its optimum is a [cycle cover of a directed graph](../../../../../cycle-cover-of-a-directed-graph.md), possibly with several disjoint cycles. Since every tour is such a cover, its cost is a [lower bound](../../../../../lower-bound-in-a-partially-ordered-set.md) on the best tour cost. This is the [assignment relaxation of the travelling salesman problem](../../../../../assignment-relaxation-of-the-travelling-salesman-problem.md).

If the minimizing cover is a single [Hamiltonian cycle](../../../../../hamilton-cycle.md), it supplies a tour and can update the incumbent. Otherwise choose one proper subtour $C$. No tour can contain all [edges](../../../../../edge-of-a-graph.md) of $C$, since that would close a cycle before visiting the remaining cities. Make one child subproblem for each [edge](../../../../../edge-of-a-graph.md) of $C$, forbidding that [edge](../../../../../edge-of-a-graph.md), and solve its modified [assignment problem](../../../../../assignment-problem.md). These branches may overlap but together retain every possible tour. Prune a child if it is infeasible or its assignment bound is at least the incumbent cost. Further subtours cause further branching. Each branch adds a new forbidden [edge](../../../../../edge-of-a-graph.md), so the search is finite, and the covering property plus the valid [lower bounds](../../../../../lower-bound-in-a-partially-ordered-set.md) proves optimality when no open branch remains. This enforces the effect of [subtour elimination constraints](../../../../../subtour-elimination-constraints.md) through [branch and bound](../../../../../branch-and-bound.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
