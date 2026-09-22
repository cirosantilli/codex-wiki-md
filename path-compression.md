# Path compression

↑ **Parent:** [Disjoint-set forest](disjoint-set-forest.md)

[Path compression](path-compression.md) changes parent pointers during a [disjoint-set find operation](disjoint-set-find-operation.md) so that future queries traverse fewer [edges](edge-of-a-graph.md). Full [path compression](path-compression.md) first follows the entire parent route to its [root of a tree](root-of-a-tree.md), then makes every member on that route point directly to that same [root of a tree](root-of-a-tree.md). No member changes its [block of a set partition](block-of-a-set-partition.md) or its [disjoint-set representative](disjoint-set-representative.md). Pointers outside the traversed route stay as they were. The following iterative Python implements full [path compression](path-compression.md) and [union by rank](union-by-rank.md); `parent` and `rank` are initially indexed [arrays](array-data-structure.md) with `parent[x] = x` and `rank[x] = 0` for every valid member.

```
def find(x):
    root = x
    while parent[root] != root:
        root = parent[root]
    while parent[x] != x:
        following = parent[x]
        parent[x] = root
        x = following
    return root

def unite(x, y):
    a, b = find(x), find(y)
    if a == b:
        return False
    if rank[a] < rank[b]:
        a, b = b, a
    parent[b] = a
    if rank[a] == rank[b]:
        rank[a] += 1
    return True
```

Starting from the displayed [disjoint-set forest](disjoint-set-forest.md), `find(3)` traverses $3\to4\to2$, returns $2$ and changes only $\mathrm{parent}[3]$ from $4$ to $2$. The route $5\to6\to2$ still has two [edges](edge-of-a-graph.md). Then `find(5)` changes only $\mathrm{parent}[5]$ from $6$ to $2$. The final parent [array](array-data-structure.md) is $(2,2,2,2,2,2,7)$; every stored rank retains its displayed value. The [rooted tree](rooted-tree.md) at $2$ now has height one although its root's rank is two. Root $7$ still represents a separate [singleton set](singleton-mathematics.md).

<a id="image-full-path-compression-shortens-two-parent-routes-while-union-by-rank-metadata-stays-unchanged"></a>
![](disjoint-set-union-path-compression-rank.png)

**[Figure 20](#image-full-path-compression-shortens-two-parent-routes-while-union-by-rank-metadata-stays-unchanged). Full path compression shortens two parent routes while union by rank metadata stays unchanged**. Arrows point towards the [parent in a rooted tree](parent-in-a-rooted-tree.md); self-pointers at roots are omitted. The same [partition of a set](partition-of-a-set.md) appears before and after `find(3)` followed by `find(5)`. Labels $r$ record stored ranks, including historical ranks at nonroots.

The two-pass [algorithm](algorithm-split.md) first discovers the answer and then reuses it. During the second pass, saving `following` before overwriting the pointer preserves the remaining route. Every replacement pointer targets the original [root of a tree](root-of-a-tree.md), proving that the [partition of a set](partition-of-a-set.md) is unchanged.

Full [path compression](path-compression.md) is one specific rule. The authored `UF.java` implementation instead uses path halving, redirecting a visited member to its parent's parent while advancing along the route. Its [union by rank](union-by-rank.md) rule agrees with the one above.[Algorithms, 4th edition by Robert Sedgewick and others; UF.java, find and union methods: halving assignment versus the full-compression algorithm here; lower-rank linking and equal-rank increment](algorithms-4th-edition-by-robert-sedgewick-and-others/uf-java.md)

## ↑ Ancestors (5)

1. [Disjoint-set forest](disjoint-set-forest.md)
2. [Disjoint-set data structure](disjoint-set-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Disjoint-set find operation](disjoint-set-find-operation.md)
- [Path compression](path-compression.md)
- [Union by rank](union-by-rank.md)
- [Union by size](union-by-size.md)
- [Union-find operation bounds](union-find-operation-bounds.md)
