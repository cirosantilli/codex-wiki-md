# Order-induced acyclic orientation

↑ **Parent:** [Acyclic orientation](acyclic-orientation.md)

Choose a [strict total order](strict-total-order.md) $v_1<\cdots<v_n$ of the [vertices](vertex-graph-theory.md) of a finite [simple graph](simple-graph.md). Direct every [edge](edge-of-a-graph.md) $v_iv_j$ from $v_i$ to $v_j$ when $i<j$. Along every [directed path](directed-path.md), the index strictly increases. Returning to the starting [vertex](vertex-graph-theory.md) would require an impossible strict increase back to the initial index, so this is an [acyclic orientation](acyclic-orientation.md). The displayed $D_1$ comes from $A<B<C$.

The chosen [strict total order](strict-total-order.md) is a [topological order](topological-order.md) of the resulting [Directed acyclic graph](directed-acyclic-graph.md). Conversely, every [acyclic orientation](acyclic-orientation.md) of a finite [simple graph](simple-graph.md) has a [topological order](topological-order.md), and orienting its [edges](edge-of-a-graph.md) from earlier to later in that order recovers it. Different [topological orders](topological-order.md) can induce the same [acyclic orientation](acyclic-orientation.md), since [vertices](vertex-graph-theory.md) with no [edge](edge-of-a-graph.md) between them need not impose a choice of arrow.[printed pp. 4–6: job scheduling, topological sorting and its edge-order correctness condition](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search.md)

An order respects [reachability](reachability-in-a-graph.md) but does not create it: $u<v$ in a chosen [topological order](topological-order.md) does not imply a [directed path](directed-path.md) from $u$ to $v$. For example, orient the two [edges](edge-of-a-graph.md) of the [graph path](path-in-a-graph.md) $A,B,C$ using $A<C<B$. The arrows are $A\to B$ and $C\to B$; there is no [directed path](directed-path.md) from $A$ to $C$, despite $A<C$. In $D_1$, however, $A$ reaches $C$ both directly and via $B$. Following outgoing [directed edges](directed-edge.md) with [graph search](graph-search.md) decides this directional [reachability](reachability-in-a-graph.md).[printed pp. 1–2: directed adjacency lists contain outgoing edges; a search sees vertices reachable from its start](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search.md)

## ↑ Ancestors (7)

1. [Acyclic orientation](acyclic-orientation.md)
2. [Orientation of a graph](orientation-of-a-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
