<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The residual [constraint graph](../../../../../constraint-graph.md) is a **[tree](../../../../../tree-graph-theory-split.md)**, rooted conveniently at $B$, with children $A,D,E$ and with $C$ a child of $A$. Solve it by the [tree-structured constraint satisfaction](../../../../../tree-structured-constraint-satisfaction.md) [algorithm](../../../../../algorithm-split.md): enforce [arc consistency](../../../../../arc-consistency.md) from children toward their parents, then choose a surviving root value and select supported child values in the opposite direction.

For adjacent agents define the combined [binary constraint](../../../../../binary-constraint.md)

$$
R_{i\ell}(X,Y)\iff
X\cap Y=\varnothing,\quad v_i(X)\ge v_i(Y),\quad
v_\ell(Y)\ge v_\ell(X).
$$

A child-to-parent [arc consistency](../../../../../arc-consistency.md) step deletes each parent bundle with no compatible child bundle. Process the [edges](../../../../../edge-of-a-graph.md) in the order $A\leftarrow C$, $B\leftarrow A$, $B\leftarrow D$, $B\leftarrow E$.

First, $C$ needs a nonempty subset of $\{1,2\}$. Supporting $C$ reduces $A$'s [constraint domain](../../../../../constraint-domain.md) to

$$
D_A'=\bigl\{\{2\},\{3\},\{1,3\},\{2,3\}\bigr\}.
$$

Indeed, $\{1\}$ leaves only $\{2\}$ for $C$ but gives $A$ value $2<3$; $\{1,2\}$ and $\{1,2,3\}$ leave no possible item for $C$. Each of the four retained choices has a compatible choice for $C$.

Next, supporting $A$ reduces $B$'s [constraint domain](../../../../../constraint-domain.md) to all nonempty subsets of $\{4,5,6,7\}$. To see why item $3$ cannot remain in $B$'s bundle, a disjoint compatible $A$ bundle from $D_A'$ would have to be $\{2\}$, but $A$ then values its own bundle at $3$ and $B$'s at least at $6$. Conversely any nonempty subset of $\{4,5,6,7\}$ is compatible with $A=\{2\}$.

Supporting $D$ next reduces $B$'s [constraint domain](../../../../../constraint-domain.md) to

$$
\bigl\{\{6\},\{7\},\{4,6\},\{4,7\},\{6,7\},\{4,6,7\}\bigr\}.
$$

If $B$ held item $5$, disjointness would force $D=\{4\}$, whose value $1$ is below $D$'s value $4$ for $B$'s bundle. If $B$ holds $4$ but not $5$, then $D=\{5\}$, and $B$ needs value at least $6$ to avoid envying $D$. If $B$ holds neither, $D=\{4\}$ supports every nonempty subset of $\{6,7\}$.

Finally, supporting $E$ leaves

$$
D_B'=\bigl\{\{6\},\{7\},\{4,6\},\{4,7\}\bigr\}.
$$

The removed choices contained both $6$ and $7$, leaving no item for $E$. Every displayed choice has a compatible choice for $E$.

Choose $B=\{6\}$, then supported child values, giving

$$
\boxed{X_A=\{2\},\quad X_B=\{6\},\quad X_C=\{1\},\quad
X_D=\{4\},\quad X_E=\{7\}.}
$$

Items $3,5$ remain unallocated, which this variant expressly permits. To check every [envy-free allocation](../../../../../envy-free-allocation.md) inequality, the matrix of agents' [additive valuations](../../../../../additive-valuation.md) of these bundles, with rows and columns both ordered $A,B,C,D,E$, is

$$
\begin{pmatrix}
3&0&2&0&0\\
0&3&0&3&3\\
1&0&1&0&0\\
0&0&0&1&0\\
0&2&0&0&2
\end{pmatrix}.
$$

Each diagonal entry is at least every entry in its row. The bundles are nonempty, pairwise disjoint, and contain only positively valued items, so all remaining requirements hold.

Why does selecting supported children suffice? The residual [constraint graph](../../../../../constraint-graph.md) has no [graph cycle](../../../../../cycle-in-a-graph.md), so different child subtrees have no constraints between them. Child-to-parent [arc consistency](../../../../../arc-consistency.md) has already ensured a compatible continuation below every retained parent value. Applying this observation recursively proves that the downward choices complete a solution without [backtracking](../../../../../backtracking.md). With $N$ variables and maximum [constraint domain](../../../../../constraint-domain.md) size $d$, the basic compatibility checks require $O(Nd^2)$ [time complexity](../../../../../time-complexity.md) in [Big O notation](../../../../../big-o-notation.md), counting each [binary constraint](../../../../../binary-constraint.md) evaluation as one operation; evaluating bundle sums has its own input-dependent cost.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
