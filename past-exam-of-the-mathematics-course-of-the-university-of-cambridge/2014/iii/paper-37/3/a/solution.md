<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use safety for failure counts within the available components, equivalently tolerance of up to that many failures. An exact-count condition with more failures than components would otherwise be vacuous. Assume the client is not itself a server; that exceptional case needs no network connection.

Create a [flow network](../../../../../../flow-network.md) by replacing each undirected link by two oppositely directed arcs of capacity one. Add a new sink $z$ and arcs from every server to $z$, each of capacity $B=|E|+1$. Find a [maximum flow](../../../../../../maximum-flow-problem.md) from $c$ to $z$ with the [Edmonds–Karp algorithm](../../../../../../edmonds-karp-algorithm.md). By the [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md), its value $\lambda$ is the minimum cut capacity. A cut using a server-to-sink arc costs at least $B$, whereas cutting all original links costs at most $|E|$, so a minimum cut uses none of the added arcs.

A source-side cut therefore contains no server. Each original undirected edge crossing it contributes exactly one of its two arcs, so its capacity is the number of original links separating the client from every server. Conversely, if a set of failed links disconnects all servers, the vertices still reachable from $c$ define a cut contained in that failed set. Thus $\lambda$ is exactly the minimum number of links whose failure can disconnect the client from all servers. This is [server connectivity under component failures](../../../../../../server-connectivity-under-component-failures.md).

Deleting fewer than $\lambda$ links leaves some connection, while deleting a minimum cut destroys every connection. Therefore

$$
\boxed{k_{\max}=\lambda-1.}
$$

If $\lambda=0$, the network is already disconnected and has no nonnegative safe failure count. The transformed graph has $|V|+1$ vertices and $2|E|+|S|$ arcs. The [Edmonds–Karp algorithm](../../../../../../edmonds-karp-algorithm.md) runs in $O(|V'||E'|^2)$ steps, so both the construction and computation are polynomial in the original graph size.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
