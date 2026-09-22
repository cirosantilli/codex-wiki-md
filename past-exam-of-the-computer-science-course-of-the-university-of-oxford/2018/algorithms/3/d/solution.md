<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Regard the two kinds of agents as the two sides of a [complete bipartite graph](../../../../../complete-bipartite-graph.md), with [edge weight](../../../../../edge-weight.md) $c_{ij}$. Pairing everyone is a [perfect matching](../../../../../perfect-matching.md), and its maximum total weight is $P$. Consider the capacitated [linear program](../../../../../linear-programming-split.md)

$$
\begin{aligned}
P_{\rm LP}=\max\quad&\sum_{i,j}c_{ij}x_{ij}\\
\text{subject to}\quad&\sum_jx_{ij}\leq1\quad(1\leq i\leq n),\\
&\sum_ix_{ij}\leq1\quad(1\leq j\leq n),\qquad x_{ij}\geq0.
\end{aligned}
$$

It is feasible and bounded. Every optimum has all row and column sums equal to one: otherwise the equal total deficits of the two sides give a row $i$ and column $j$ both below one. Increasing $x_{ij}$ by the smaller of their positive deficits remains feasible and increases the objective because $c_{ij}>0$, a contradiction.

Thus an optimum is a [doubly stochastic matrix](../../../../../doubly-stochastic-matrix.md). By the [Birkhoff-von Neumann theorem](../../../../../birkhoff-von-neumann-theorem.md) it is a [convex combination](../../../../../convex-combination.md) of [permutation matrices](../../../../../permutation-matrix.md), so at least one corresponding [perfect matching](../../../../../perfect-matching.md) has weight at least its objective. Conversely every such [perfect matching](../../../../../perfect-matching.md) gives a feasible [matrix](../../../../../matrix.md). Hence $P_{\rm LP}=P$. One way to justify the decomposition is to apply [Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) to the positive-entry support, subtract the smallest entry on a supported [perfect matching](../../../../../perfect-matching.md), and repeat after rescaling the nonzero remainder; each subtraction removes a positive entry, so the process terminates.

The [dual linear program](../../../../../dual-linear-program.md) assigns nonnegative [dual variables](../../../../../dual-variable.md) $p_i,q_j$ to the row and column capacity constraints:

$$
\boxed{\min\sum_i p_i+\sum_jq_j\quad\text{subject to}\quad p_i+q_j\geq c_{ij},\qquad p_i,q_j\geq0.}
$$

These are exactly the permitted payments and all the pairwise acceptance conditions, so its optimal value is $Q$. It is feasible, for example by taking $p_i=\max_jc_{ij}$ and $q_j=0$. [Strong duality](../../../../../strong-duality.md) now gives **$P=P_{\rm LP}=Q$**. In particular, the nonnegative payment restriction has been retained throughout; using capacity inequalities rather than equality constraints avoids introducing unrestricted prices.

For a direct [weak duality](../../../../../weak-duality.md) check, sum $p_i+q_{\pi(i)}\geq c_{i,\pi(i)}$ over any pairing $\pi$. Its revenue never exceeds the company's total offered payment. The [linear programming duality](../../../../../linear-programming-duality.md) and integrality argument prove that this lower bound on payments is attained.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
