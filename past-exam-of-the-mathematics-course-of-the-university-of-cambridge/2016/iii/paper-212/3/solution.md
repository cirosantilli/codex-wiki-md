<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a directed [bipartite graph](../../../../../bipartite-graph.md) with one vertex for each job and one for each agent. Job vertices have supply $1$ and agent vertices demand $1$. An arc from job $i$ to agent $j$ has cost $c_{ij}$ and nonnegative flow $x_{ij}$; an upper bound $1$ may be added, but is already implied by the balances. The **[minimum-cost flow](../../../../../minimum-cost-flow-problem.md) formulation of the [assignment problem](../../../../../assignment-problem.md)** is

$$
\boxed{\min\sum_{i,j}c_{ij}x_{ij},\qquad \sum_jx_{ij}=1,\quad\sum_ix_{ij}=1,\quad x_{ij}\geq0.}
$$

Integer supplies and demands give an integral optimum by [integrality of the transportation problem](../../../../../integrality-of-the-transportation-problem.md). Its $n$ positive arcs form a [perfect matching](../../../../../perfect-matching.md), hence give one job per agent.

A [network simplex algorithm](../../../../../network-simplex-algorithm.md) basis for this connected $2n$-vertex network has $2n-1$ tree arcs, whereas an integral assignment has only $n$ positive flows. For $n>1$, at least $n-1$ basic tree arcs therefore carry zero flow. This unavoidable **[degeneracy in linear programming](../../../../../degeneracy-in-linear-programming.md)** can cause zero-step pivots, extra bookkeeping and cycling unless an appropriate pivot rule is used. The [Hungarian algorithm](../../../../../hungarian-algorithm.md) exploits the assignment structure directly rather than maintaining many zero-flow basic arcs.

Suppose the [assignment dual potentials](../../../../../assignment-dual-potentials.md) satisfy $\lambda_i-\mu_j\leq c_{ij}$. For every feasible assignment $y$,

$$
\sum_{i,j}c_{ij}y_{ij}\geq\sum_{i,j}(\lambda_i-\mu_j)y_{ij}=\sum_i\lambda_i-\sum_j\mu_j.
$$

If the selected assignment $x$ uses only arcs with $\lambda_i-\mu_j=c_{ij}$, its cost equals this lower bound. **[Weak duality](../../../../../weak-duality.md) and [complementary slackness](../../../../../complementary-slackness.md) certify optimality.** The PDF correctly denotes the feasible assignment by $x_{ij}$; the TeX aid mistakenly replaces it with $\lambda_{ij}$.

The [Hungarian algorithm](../../../../../hungarian-algorithm.md) maintains feasible [assignment dual potentials](../../../../../assignment-dual-potentials.md) and a [matching in a graph](../../../../../matching-graph-theory.md) of zero [reduced cost](../../../../../reduced-cost.md) edges, where $r_{ij}=c_{ij}-\lambda_i+\mu_j\geq0$. Search for an [augmenting path in a matching](../../../../../augmenting-path-in-a-matching.md) in this equality graph. If there is none, let $S$ be the reachable jobs and $T$ the reachable agents in the alternating search from unmatched jobs. Every agent in $T$ is matched to a job in $S$. Set

$$
\Delta=\min_{i\in S,\ j\notin T}r_{ij}>0,\qquad \lambda_i\leftarrow\lambda_i+\Delta\ (i\in S),\quad \mu_j\leftarrow\mu_j+\Delta\ (j\in T).
$$

[Reduced costs](../../../../../reduced-cost.md) from $S$ to its complement decrease by $\Delta$, those from outside $S$ into $T$ increase, and the remaining ones do not change. Thus feasibility and current matching equalities are preserved, while at least one new equality edge appears. Continue until an [augmenting path in a matching](../../../../../augmenting-path-in-a-matching.md) increases the matching size. A [perfect matching](../../../../../perfect-matching.md) in the equality graph then has the same value as the [dual linear program](../../../../../dual-linear-program.md) and is optimal.

For the example, start with the row minima $\lambda=(10,50,50)$ and $\mu=(0,0,0)$. The [reduced cost](../../../../../reduced-cost.md) matrix is

$$
R^{(0)}=\begin{pmatrix}0&25&40\\0&20&10\\0&30&25\end{pmatrix}.
$$

Match job $1$ to agent $1$. Searching from both unmatched jobs gives $S=\{1,2,3\}$ and $T=\{1\}$; the minimum cost to an agent outside $T$ is $\Delta=10$. Update to $\lambda=(20,60,60)$ and $\mu=(10,0,0)$:

$$
R^{(1)}=\begin{pmatrix}0&15&30\\0&10&0\\0&20&15\end{pmatrix}.
$$

The new equality edge $(2,3)$ augments the matching. From unmatched job $3$, the next alternating search reaches agent $1$ and its matched job $1$, giving $S=\{1,3\}$ and $T=\{1\}$. Now $\Delta=15$. The updated feasible [assignment dual potentials](../../../../../assignment-dual-potentials.md) and [reduced costs](../../../../../reduced-cost.md) are

$$
\lambda=(35,60,75),\qquad\mu=(25,0,0),\qquad R^{(2)}=\begin{pmatrix}0&0&15\\15&10&0\\0&5&0\end{pmatrix}.
$$

The [augmenting path in a matching](../../../../../augmenting-path-in-a-matching.md) $J_3\to A_1\to J_1\to A_2$ uses job $3$ to agent $1$, the reversed matched edge to job $1$, then the new edge to agent $2$. It gives **the optimal assignment**

$$
\boxed{1\mapsto2,\quad2\mapsto3,\quad3\mapsto1,\qquad \text{minimum cost}=35+60+50=145.}
$$

The [dual linear program](../../../../../dual-linear-program.md) value is $35+60+75-25=145$, an independent optimality certificate.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
