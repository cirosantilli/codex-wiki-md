<h1 id="d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

For an undirected [graph](../../../../graph-split.md) with [adjacency matrix](../../../../adjacency-matrix.md) $A$, [degrees of vertices](../../../../degree-graph-theory.md) $k_i$ and $m$ edges, [network modularity](../../../../network-modularity.md) is

$$
Q=\frac{1}{2m}\sum_{C}\sum_{i,j\in C}
\left(A_{ij}-\frac{k_i k_j}{2m}\right).
$$

Each undirected edge contributes twice to the double sum, explaining the denominator $2m$. Include the terms with $i=j$: even though the observed graph has no self-loops, the null-model contribution on the diagonal is part of this definition.

An independent implementation forms the modularity matrix and sums its within-community blocks. Initializing the best value to negative infinity also handles a candidate collection whose scores are all negative:

```
def modularity(adjacency,communities):
    a=np.asarray(adjacency);degrees=a.sum(axis=1);twom=degrees.sum()
    if twom==0:raise ValueError('positive edge count required')
    B=a-np.outer(degrees,degrees)/twom
    return sum(B[np.ix_(group,group)].sum() for group in communities)/twom

best_score = -np.inf
best_partition = None
for candidate in community_partitions:
    value = modularity(adjacency_matrix, candidate)
    if value > best_score:
        best_score, best_partition = value, candidate
print(best_partition, best_score)
```

**The best partition is $\boxed{\{0,1,2\}\mid\{3,4,5\}}$, with $\boxed{Q=5/14\simeq0.357143}$.** There are seven edges, and each selected community has three internal edges and total degree seven, so independently

$$
Q=2\left(\frac{3}{7}-\left(\frac{7}{14}\right)^2\right)=\frac5{14}.
$$

The supplied candidates include the optimum, but do not exhaust even the balanced two-community [set partitions](../../../../set-partition.md): there are $\binom{5}{2}=10$ of those, rather than six. To substantiate a best partition among all community counts, the following short recursion enumerates all 203 unlabeled [set partitions](../../../../set-partition.md) of the six vertices:

```
def partitions(items):
    if not items:
        yield [];return
    first,*rest=items
    for part in partitions(rest):
        yield [[first]]+[g.copy() for g in part]
        for j in range(len(part)):
            new=[g.copy() for g in part];new[j]=[first]+new[j];yield new

candidates = list(partitions(list(range(len(adjacency_matrix)))))
best_partition = max(candidates, key=lambda p: modularity(adjacency_matrix, p))
print(len(candidates), best_partition, modularity(adjacency_matrix, best_partition))
```

This exhaustive calculation returns the same two triangles and the same [network modularity](../../../../network-modularity.md). Enumerating every [set partition](../../../../set-partition.md) becomes impractical rapidly as the number of vertices increases, but is small enough here to verify the global optimum.

## ↑ Ancestors (12)

1. [D12](../d12.md)
2. [Paper 2](../../paper-2-split.md)
3. [2024](../../split.md)
4. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../split.md)
5. [Mathematical and Computational Biology course of the University of Cambridge](../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
