<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $A\subseteq E$, write $x(A)=\sum_{e\in A}x_e$, and let $\kappa(A)$ count the connected components of $(V,A)$, including isolated vertices. A maximal [forest](../../../../forest.md) in each component has one fewer [edge](../../../../edge-of-a-graph.md) than vertices, so $r(A)=|V|-\kappa(A)$. The required [forest polytope](../../../../forest-polytope.md) is

$$
\boxed{P=\{x\in\mathbb R^E:x_e\geq0\ (e\in E),\quad x(A)\leq |V|-\kappa(A)\ (A\subseteq E)\}.}
$$

We prove both inclusions, using the [matroid independence polytope](../../../../matroid-independence-polytope.md) argument explicitly.

If $I$ is a [forest](../../../../forest.md), $I\cap A$ is an independent [subset](../../../../subset.md) of $A$, so $\mathbf1_I(A)=|I\cap A|\leq r(A)$. Its indicator is nonnegative. All [convex combinations](../../../../convex-combination.md) of these indicators therefore lie in $P$.

For the converse, take any real objective vector $c$. List just its positive-weight [edges](../../../../edge-of-a-graph.md) as $e_1,\ldots,e_k$ with $c_1\geq\cdots\geq c_k>0$, put $c_{k+1}=0$, and set $S_i=\{e_1,\ldots,e_i\}$. Run the [forest](../../../../forest.md) greedy [algorithm](../../../../algorithm-split.md) on these [edges](../../../../edge-of-a-graph.md) and call the output $I$. At every prefix, the accepted [edges](../../../../edge-of-a-graph.md) form a maximal [forest](../../../../forest.md) of $(V,S_i)$, so

$$
|I\cap S_i|=r(S_i).
$$

Indeed a previously rejected [edge](../../../../edge-of-a-graph.md) still has its endpoints joined later; therefore no rejected prefix [edge](../../../../edge-of-a-graph.md) can augment the chosen [forest](../../../../forest.md). A maximal [forest](../../../../forest.md) spans every prefix component and has the stated size.

For every $x\in P$, dropping nonpositive objective terms and telescoping now gives

$$
\begin{aligned}
c^Tx
&\leq\sum_{j=1}^kc_jx_{e_j}
=\sum_{i=1}^k(c_i-c_{i+1})x(S_i)\\
&\leq\sum_{i=1}^k(c_i-c_{i+1})r(S_i)
=c^T\mathbf1_I.
\end{aligned}
$$

The last equality uses the same telescoping identity for the greedy indicator. If there are no positive coefficients, the empty [forest](../../../../forest.md) attains the bound zero. Thus **every linear objective over $P$ is maximized by a [forest](../../../../forest.md) indicator**.

The [singleton](../../../../singleton-mathematics.md) inequalities give $0\leq x_e\leq r(\{e\})\leq1$, so $P$ is [compact](../../../../compact-space.md). The [convex hull](../../../../convex-hull.md) $Q$ of the finitely many [forest](../../../../forest.md) indicators is also [compact](../../../../compact-space.md). If some $x\in P$ were outside $Q$, the finite-dimensional [separating hyperplane theorem](../../../../hyperplane-separation-theorem.md) would give $c$ with $c^Tx>\max_{y\in Q}c^Ty$, contradicting the bound just proved. Therefore $P\subseteq Q$, completing the convex-hull proof.

An equivalent system indexed by vertex sets is

$$
\boxed{x_e\geq0,\qquad x(E(S))\leq |S|-1\quad(\varnothing\ne S\subseteq V),}
$$

where $E(S)$ contains all [edges](../../../../edge-of-a-graph.md) with both ends in $S$. The rank system implies this since $r(E(S))\leq|S|-1$. Conversely, split any [edge](../../../../edge-of-a-graph.md) set $A$ into its vertex components $S_1,\ldots,S_t$. Nonnegativity and the vertex inequalities give $x(A)\leq\sum_jx(E(S_j))\leq\sum_j(|S_j|-1)=|V|-\kappa(A)$. Hence this second system describes the same polytope.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
