<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Compute any [topological sort](../../../../../topological-sorting.md) $(w_1,\ldots,w_n)$ using a standard algorithm, then check its consecutive entries in the [adjacency matrix](../../../../../adjacency-matrix.md):
```
DAGHamiltonianPath(A):
    order = TopologicalSort(A)
    for j = 1,...,n-1:
        if not A[order[j],order[j+1]]:
            return "no Hamiltonian path"
    return order
```
If all checks pass, the returned ordering is a [Hamiltonian path](../../../../../hamiltonian-path.md). If a check fails but a [Hamiltonian path](../../../../../hamiltonian-path.md) existed, part (d) would force the computed [topological sort](../../../../../topological-sorting.md) to equal the unique path order, whose consecutive edges all exist. This contradiction proves the negative answer correct.

A standard [topological sort](../../../../../topological-sorting.md) scans all matrix rows and therefore takes $O(n^2)$ time with this input representation; the subsequent $n-1$ edge checks take $O(n)$. The answer is consequently **$O(n^2)$ time**, with $O(n)$ auxiliary storage beyond the input matrix. An $O(|V|+|E|)$ bound for an [adjacency list](../../../../../adjacency-list.md) must not be substituted for the stipulated [adjacency matrix](../../../../../adjacency-matrix.md) bound.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
