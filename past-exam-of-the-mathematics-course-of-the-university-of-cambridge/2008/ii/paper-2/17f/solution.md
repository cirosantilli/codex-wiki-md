<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Here graphs are finite and simple. To prove [Dirac theorem](../../../../../dirac-s-theorem.md), take a longest path $v_1,\ldots,v_\ell$. All neighbours of either endpoint lie on the path. Among indices $1\le i<\ell$, let $S=\{i:v_1v_{i+1}\text{ is an edge}\}$ and $T=\{i:v_iv_\ell\text{ is an edge}\}$. Since $|S|+|T|=d(v_1)+d(v_\ell)\ge n>\ell-1$, some $i$ lies in both. Following the path forward to $v_i$, jumping to $v_\ell$, and following it backwards to $v_{i+1}$ closes a cycle containing every vertex of the path. The degree condition makes the graph connected: two components would each have at least $\delta+1>n/2$ vertices. If $\ell<n$, connectedness gives an edge from an outside vertex to the cycle, and breaking the cycle there makes a longer path. This contradiction proves a [Hamiltonian cycle](../../../../../hamilton-cycle.md).

For even $n=2m$, the [complete bipartite graph](../../../../../complete-bipartite-graph.md) $K_{m-1,m+1}$ has minimum degree $m-1$ and no [Hamiltonian cycle](../../../../../hamilton-cycle.md). For odd $n=2m+1$, $K_{m,m+1}$ has minimum degree $m$ and likewise fails: a bipartite cycle uses equal numbers from its two parts. These examples include the smallest applicable $n$.

Adding one universal vertex gives $n+1$ vertices and minimum degree at least $(n+1)/2$ when the original minimum degree is at least $(n-1)/2$. Apply the proved theorem and remove the universal vertex from its cycle. The remaining sequence is a [Hamiltonian path](../../../../../hamiltonian-path.md) in the original graph.

A necessary condition for a [Hamiltonian cycle](../../../../../hamilton-cycle.md) is that deleting a nonempty vertex set $S$ leaves at most $|S|$ components, since deleting those vertices breaks a spanning cycle into at most that many path pieces. For any $k\ge1$, take the connected star $G=K_{1,k+2}$. In $G_k$, deleting its center and the $k$ new vertices leaves $k+2$ components, more than $k+1$. Even two-connectivity does not suffice: take $G=K_{2,k+3}$, which is two-connected. Deleting its two-vertex part and the $k$ new vertices from $G_k$ leaves $k+3$ components, more than $k+2$. **Both connectivity requirements admit counterexamples for every $k$.**

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
