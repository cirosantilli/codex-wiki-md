<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Repeatedly remove vertices whose current degree is less than $k$. Implement the deletions with an [adjacency list](../../../../../adjacency-list.md), a queue and a degree counter for each active vertex:
```
active[v] = True for every v
count[v] = degree(v)
queue all v with count[v] < k
while the queue is nonempty:
    remove v from the queue
    if not active[v]: continue
    active[v] = False
    for each neighbour u of v:
        if active[u]:
            count[u] -= 1
            if count[u] == k-1: queue u
return the subgraph induced by the active vertices,
       or report failure if there is no active vertex
```
The requested subgraph is understood to be nonempty; otherwise an empty output would make the degree requirement vacuous or undefined. For $k\leq0$, any nonempty input graph already qualifies.

The correctness [invariant](../../../../../invariant-mathematics.md) is that every subgraph with minimum degree at least $k$ has all its vertices still active. Initially this is immediate. When $v$ is deleted, its degree in the whole active [induced subgraph](../../../../../induced-subgraph.md) is less than $k$. Any candidate subgraph on active vertices has at most that many incident edges at $v$, so cannot contain it. Thus the invariant survives every deletion.

At termination, every active vertex has current degree at least $k$, since every counter initially below the threshold or subsequently crossing it was queued. A nonempty surviving induced subgraph is therefore a valid answer. If none survives, the invariant rules out every possible answer, including ones omitting additional edges. The result is the [k-core](../../../../../k-core.md), with the [k-core peeling invariant](../../../../../k-core-peeling-invariant.md) proving that deletion order cannot destroy a valid solution.

Each vertex is enqueued at most once when initially deficient or first crossing the threshold. Each adjacency list is scanned once when its vertex is deleted. The running time is **$O(|V|+|E|)$**, and storage is $O(|V|+|E|)$ including the input graph.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
