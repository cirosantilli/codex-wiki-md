# Topological order

↑ **Parent:** [Topological sorting](topological-sorting.md)

A [topological order](topological-order.md) of a finite [directed graph](directed-graph.md) $G=(V,E)$ is a [sequence](sequence.md) $(v_1,\ldots,v_n)$ containing every [vertex](vertex-graph-theory.md) exactly once, with

$$
(v_i,v_j)\in E\quad\Longrightarrow\quad i<j.
$$

Thus every [directed edge](directed-edge.md) points forward in the list. Equivalently, a [bijection](bijection.md) $p:V\to\{1,\ldots,n\}$ assigning positions satisfies $p(u)<p(v)$ for every [directed edge](directed-edge.md) $u\to v$. A [topological ordering](topological-ordering.md) names the same kind of list. [MIT, Recitation 10, p. 3: the edge-by-edge definition](https://live.ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/d9265b3b33d238ff914b0223ac8e7628_MIT6_006S20_r10.pdf)

The toy [Directed acyclic graph](directed-acyclic-graph.md) has exactly five [topological orders](topological-order.md): $ABCDE$, $ABDCE$, $ACBDE$, $BACDE$, and $BADCE$. These lists were checked by enumerating all $5!=120$ [permutations](permutation.md) and retaining precisely those satisfying all five [directed edge](directed-edge.md) inequalities. Every list ends with $E$, since all other tasks have a [directed path](directed-path.md) to publication. A [topological order](topological-order.md) need not put adjacent entries next to one another in the [directed graph](directed-graph.md): $A$ and $B$ are consecutive in $ABCDE$ without a [directed edge](directed-edge.md) between them.

A [directed cycle](directed-cycle.md) would force the impossible chain of position inequalities $p(u_1)<p(u_2)<\cdots<p(u_k)<p(u_1)$. In the toy example, adding $E\to C$ requires review before publication and publication before review, so there are no [topological orders](topological-order.md). Together with the construction in [topological sorting](topological-sorting.md), this proves that a finite [directed graph](directed-graph.md) admits a [topological order](topological-order.md) if and only if it is a [Directed acyclic graph](directed-acyclic-graph.md). The empty [directed graph](directed-graph.md) has the empty [sequence](sequence.md) as its [topological order](topological-order.md).

There is also a useful connection to [partial orders](partially-ordered-set.md): define $u\preceq v$ when $u=v$ or there is a [directed path](directed-path.md) from $u$ to $v$. For a [Directed acyclic graph](directed-acyclic-graph.md), this [reachability](reachability-in-a-graph.md) relation is a [partial order](partially-ordered-set.md), and its [linear extensions](linear-extension.md) are exactly the [topological orders](topological-order.md). The [Directed acyclic graph](directed-acyclic-graph.md) specifies which pairs must be ordered; a [topological order](topological-order.md) chooses positions for all the remaining pairs.

## ↑ Ancestors (6)

1. [Topological sorting](topological-sorting.md)
2. [Directed acyclic graph](directed-acyclic-graph.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Cached cell value](cached-cell-value.md)
- [Critical path method](critical-path-method.md)
- [Directed acyclic graph](directed-acyclic-graph.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/2/solution.md)
- [Project scheduling](project-scheduling.md)
- [Spreadsheet circular reference](spreadsheet-circular-reference.md)
- [Spreadsheet dependency evaluation](spreadsheet-dependency-evaluation.md)
- [Topological order](topological-order.md)
- [Topological ordering](topological-ordering.md)
- [Topological sorting](topological-sorting.md)
