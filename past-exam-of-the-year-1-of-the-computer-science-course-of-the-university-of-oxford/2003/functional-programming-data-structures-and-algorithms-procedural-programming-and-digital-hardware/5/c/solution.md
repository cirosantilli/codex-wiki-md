<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [DAG shortest-path algorithm](../../../../../dag-shortest-path-algorithm.md): first compute a [topological ordering](../../../../../topological-ordering.md), then perform [edge relaxation](../../../../../edge-relaxation.md) once for every edge in that order. Store a [shortest-path predecessor](../../../../../shortest-path-predecessor.md) when a distance improves so that the actual paths, as well as their costs, can be recovered.

```
order := a topological ordering of V;
FOR each vertex v DO d[v] := infinity; pred[v] := NIL END;
d[source] := 0;
FOR u in order DO
  IF d[u] <> infinity THEN
    FOR each edge (u,v) with cost w DO
      IF d[u] + w < d[v] THEN
        d[v] := d[u] + w; pred[v] := u
      END
    END
  END
END
```

Each loop has a natural invariant. During initialization, all vertices already processed have infinite distance and no predecessor. During the outer relaxation loop, all processed vertices have their final [shortest-path distances](../../../../../shortest-path-distance.md), and every edge leaving a processed vertex has been relaxed. During an inner edge loop, the outgoing edges of `u` already inspected have been relaxed using its final distance, while the outer invariant remains true for all earlier vertices.

For correctness, every path to a vertex $v$ ends with an edge $uv$ from an earlier vertex in the [topological ordering](../../../../../topological-ordering.md). When $v$ is reached, all those earlier distances are correct and all incoming edges have been relaxed. Therefore

$$
\boxed{d(v)=\min_{uv\in E}\bigl(d(u)+w(u,v)\bigr),\qquad d(s)=0,}
$$

with infinite distance for unreachable vertices and the empty path included at the source. No directed path can return to the source in a [Directed acyclic graph](../../../../../directed-acyclic-graph.md). [Induction](../../../../../mathematical-induction.md) over the [topological ordering](../../../../../topological-ordering.md) proves all distances correct. Following predecessor links backward reconstructs each reachable [shortest path](../../../../../shortest-path.md).

With [adjacency lists](../../../../../adjacency-list.md), [topological sorting](../../../../../topological-sorting.md) takes $O(|V|+|E|)$ time and the relaxation pass has the same bound, using $O(|V|)$ extra space beyond the input. Thus the full distance and predecessor representation costs $O(|V|+|E|)$ time. Printing every source-to-vertex path separately can take more time because their total output length may be quadratic. The stipulated nonnegative costs are sufficient; this [algorithm](../../../../../algorithm-split.md) actually also permits negative costs because there are no directed [graph cycles](../../../../../cycle-in-a-graph.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
