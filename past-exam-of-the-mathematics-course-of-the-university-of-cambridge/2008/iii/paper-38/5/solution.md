<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use a complete [directed graph](../../../../../directed-graph.md) on $n\geq3$ cities, with integral arc costs $c_{ij}$ and a threshold $L$. A symmetric cost matrix also represents the undirected [travelling salesman problem](../../../../../travelling-salesman-problem.md) by orienting a tour. Let the binary variable $x_{ij}$ indicate that city $j$ follows city $i$, and forbid self-arcs. The decision [integer programming](../../../../../integer-programming.md) formulation asks whether the following system has a solution:

$$
\begin{gathered}
x_{ij}\in\{0,1\}\quad(i\ne j),\\
\sum_{j\ne i}x_{ij}=1\quad(i=1,\ldots,n),\qquad
\sum_{i\ne j}x_{ij}=1\quad(j=1,\ldots,n),\\
\sum_{\substack{i,j\in S\\i\ne j}}x_{ij}\leq|S|-1
\quad(\varnothing\ne S\subsetneq\{1,\ldots,n\}),\\
\sum_{i\ne j}c_{ij}x_{ij}\leq L.
\end{gathered}
$$

The in-degree and out-degree equations make the selected arcs a [cycle cover of a directed graph](../../../../../cycle-cover-of-a-directed-graph.md). Any proper [graph cycle](../../../../../cycle-in-a-graph.md) on a city set $S$ would violate its subset inequality, so the selected arcs form one [Hamiltonian cycle](../../../../../hamilton-cycle.md). Conversely, a [Hamiltonian cycle](../../../../../hamilton-cycle.md) obeys every inequality: a proper subset cannot contain all the successor arcs of its [graph vertices](../../../../../vertex-graph-theory.md). Thus the binary feasibility system is equivalent to the decision [travelling salesman problem](../../../../../travelling-salesman-problem.md). The subset formulation has exponentially many inequalities, which is harmless for this formulation; verifying a proposed tour does not require listing them.

To call this decision problem [NP-complete](../../../../../np-completeness.md) means two separate things. It belongs to [NP](../../../../../np-complexity.md): a yes-instance has a polynomial-length [certificate in computational complexity](../../../../../certificate-complexity.md), namely the cyclic ordering of the cities, and a deterministic algorithm checks distinct visits, the return to the start, and the total cost in [polynomial time](../../../../../polynomial-time.md) in the binary input length. It is also [NP-hard](../../../../../np-hardness.md): every decision problem in [NP](../../../../../np-complexity.md) has a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) to it, preserving yes and no answers. This is a statement about worst-case computation on finite encodings, not a proof that every individual tour is hard to find or that no polynomial algorithm exists; that last conclusion would require $\mathrm P\ne\mathrm{NP}$.

For the strict-threshold decision [Max-TSP](../../../../../max-tsp.md), choose an integer $M\geq\max_{i\ne j}c_{ij}$ and replace each arc cost by $c'_{ij}=M-c_{ij}\geq0$. Every tour uses exactly $n$ arcs, so

$$
C'=nM-C,\qquad
C\leq L\ \Longleftrightarrow\ C'\geq nM-L
\ \Longleftrightarrow\ C'>nM-L-1.
$$

Set the new threshold to $L'=nM-L-1$. Its encoding length, the transformed matrix's encoding length and the computation time are all polynomial in the original input length. If thresholds are required to be nonnegative, take $M\geq\max(0,\max c_{ij},L+1)$; the same identity works. Symmetry of costs is preserved. This is a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) from decision [travelling salesman problem](../../../../../travelling-salesman-problem.md) to decision [Max-TSP](../../../../../max-tsp.md), so the latter is [NP-hard](../../../../../np-hardness.md). A tour is again a polynomially verifiable [certificate in computational complexity](../../../../../certificate-complexity.md), now checking strict excess over $L'$, so

$$
\boxed{\text{decision Max-TSP is NP-complete}.}
$$

For the [approximation algorithm](../../../../../approximation-algorithm.md), use the standard nonnegative-length setting on a complete [graph](../../../../../graph-split.md); no [triangle inequality](../../../../../triangle-inequality.md) is required. Solve the maximum-weight [assignment problem](../../../../../assignment-problem.md) with diagonal assignments forbidden, for example by applying the [Hungarian algorithm](../../../../../hungarian-algorithm.md) to the negative weights. The resulting [cycle cover of a directed graph](../../../../../cycle-cover-of-a-directed-graph.md) has weight $W$ with $W\geq\operatorname{OPT}$, since every tour is an allowed assignment.

If it already has a single [graph cycle](../../../../../cycle-in-a-graph.md), it is an optimal tour. Otherwise remove a least-weight arc from each [graph cycle](../../../../../cycle-in-a-graph.md). A [graph cycle](../../../../../cycle-in-a-graph.md) of $r\geq2$ arcs and weight $W_r\geq0$ loses at most $W_r/r\leq W_r/2$. The remaining arcs form vertex-disjoint [graph paths](../../../../../path-in-a-graph.md) covering all cities. Join the endpoint of each [graph path](../../../../../path-in-a-graph.md) to the start of the next, cyclically. The required arcs exist by completeness, and their nonnegative weights cannot diminish the retained weight. The resulting single [Hamiltonian cycle](../../../../../hamilton-cycle.md) therefore satisfies

$$
\boxed{\operatorname{ALG}\geq\frac W2\geq\frac{\operatorname{OPT}}2.}
$$

The [Hungarian algorithm](../../../../../hungarian-algorithm.md) takes $O(n^3)$ arithmetic operations, and finding the [graph cycles](../../../../../cycle-in-a-graph.md), cutting them and patching the [graph paths](../../../../../path-in-a-graph.md) takes $O(n)$ further operations. For rational or integer weights these operations have polynomial encoding length, giving [polynomial time](../../../../../polynomial-time.md). With symmetric costs, the same directed construction is a valid undirected tour after forgetting its orientation. This is the [cycle-cover patching half-approximation for Max-TSP](../../../../../cycle-cover-patching-half-approximation-for-max-tsp.md).

Nonnegativity is essential to this multiplicative guarantee. If arbitrary signed weights were allowed, giving every arc cost $-1$ would make every tour have weight $-n$, while half the optimum is $-n/2$. No tour could achieve the requested bound. Thus “length” has its usual nonnegative meaning in the approximation assertion.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
