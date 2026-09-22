<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Given a feasible [network flow](../../../../../flow.md) $f$, an original [directed edge](../../../../../directed-edge.md) $(u,v)$ has forward residual capacity $c_{uv}-f_{uv}$ and a reverse residual arc of capacity $f_{uv}$. A source–sink [graph path](../../../../../path-in-a-graph.md) in this [residual network](../../../../../residual-network.md) permits an augmentation by the minimum residual capacity along it: increase forward flows and decrease the corresponding reversed flows. Capacities and [flow conservation](../../../../../flow-conservation.md) are preserved, and the flow value increases by that amount.

If no residual source–sink [graph path](../../../../../path-in-a-graph.md) exists, let $S$ be the [vertices](../../../../../vertex-graph-theory.md) reachable from the source. The sink is outside $S$. Every original arc from $S$ to its complement is saturated, and every original arc back into $S$ has zero flow, since a positive reverse residual arc would make its tail reachable. Conservation therefore gives

$$
|f|=\sum_{u\in S,\ v\notin S}f_{uv}
-\sum_{u\notin S,\ v\in S}f_{uv}
=\sum_{u\in S,\ v\notin S}c_{uv}.
$$

The flow equals this [cut capacity](../../../../../cut-capacity.md), so the [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) proves it is [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md).

Termination needs a capacity or path-selection assumption. For [integer](../../../../../integer.md) capacities, starting from zero, every residual capacity and augmentation is integral; each augmentation increases the value by at least one, and the value is bounded by the total source-outgoing capacity. The algorithm therefore terminates. Rational capacities can be scaled to [integers](../../../../../integer.md). With arbitrary real capacities, unrestricted [graph path](../../../../../path-in-a-graph.md) choices do not guarantee finite termination. A valid uniformly terminating implementation is the [Edmonds–Karp algorithm](../../../../../edmonds-karp-algorithm.md), choosing a shortest residual [graph path](../../../../../path-in-a-graph.md) each time.

Here is why that choice works independently of numerical capacity sizes. Residual distances from the source cannot decrease after augmenting along a shortest [graph path](../../../../../path-in-a-graph.md). Every newly created residual arc is the reverse of a [graph path](../../../../../path-in-a-graph.md) arc; if it could cause the first distance decrease, its previous distance relation would contradict that decrease. When an arc $(u,v)$ is saturated on a shortest [graph path](../../../../../path-in-a-graph.md), $d(v)=d(u)+1$. Before the same direction can be saturated again, it must have been restored by a reverse augmentation on a shortest [graph path](../../../../../path-in-a-graph.md), at which time $d'(u)=d'(v)+1\geq d(v)+1=d(u)+2$. Each arc is consequently critical only $O(|N|)$ times. There are $O(|A|)$ arcs and each augmentation saturates at least one, giving $O(|N||A|)$ augmentations, each found by [Breadth-first search](../../../../../breadth-first-search.md) in $O(|A|)$ time. Thus the shortest-path Ford–Fulkerson implementation terminates and finds a [maximum flow](../../../../../maximum-flow-problem.md) in $O(|N||A|^2)$ arithmetic operations.

For [sports elimination by maximum flow](../../../../../sports-elimination-by-maximum-flow.md), first give the target team all its remaining wins. This cannot hurt its chance to finish strictly ahead: changing a result to favour it also removes a rival's win. Let $w^*$ be its resulting win count. If any rival already has at least $w^*$ wins, strict victory is impossible. Otherwise give each unordered pair of rivals $i<j<n$ one game node. Its incoming capacity is $g_{ij}$, and its two outgoing arcs go to the participating team nodes. Their capacities may be replaced by the finite number

$$
G=\sum_{i<j<n}g_{ij},
$$

since no arc can need more than the total number of remaining rival games. Team $i$ has sink capacity $w^*-w_i-1$.

An integral flow of value $G$ saturates all game-node incoming arcs. Its two outgoing amounts allocate exactly $g_{ij}$ wins to the two teams; the team-sink caps keep each rival strictly below $w^*$. Conversely any successful completion of the league specifies such a flow. Integral capacities and augmentation give an integral [maximum flow](../../../../../maximum-flow-problem.md), so

$$
\boxed{\text{the target can win strictly }
\Longleftrightarrow\text{ the maximum flow has value }G,}
$$

after the initial negative-capacity rejection. Each actual game is counted once: making independent nodes for both ordered pairs would double-count it.

The network has $O(n^2)$ nodes and arcs. If each input [integer](../../../../../integer.md) has at most $k$ bits, its derived capacities have $O(k+\log n)$ bits. The shortest-path algorithm above uses $O(n^6)$ arithmetic operations, each on [integers](../../../../../integer.md) of polynomial bit length. Therefore **the [decision problem](../../../../../decision-problem.md) belongs to P, even with $k$ part of the input**. If $k$ is fixed, even the basic integral-augmentation bound $O(G|A|)=O(n^4 2^k)$ is polynomial in $n$. If $k$ varies, that particular bound is only pseudopolynomial; it is the shortest-path implementation that establishes polynomial bit complexity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
