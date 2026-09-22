<h1 id="8/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Read “subsequence” in its usual sense: selected indices increase in the given input order. First sort each box's dimension vector, in $O(nd\log d)$ total time. Let $F[j]$ be the maximum number of boxes in a fitting [subsequence](../../../../../../subsequence.md) ending at index $j$. Process $j=1,\ldots,n$ and compute

$$
F[j]=1+\max\bigl(\{F[i]:i<j,\ a_{i,r}<a_{j,r}\text{ for every }1\le r\le d\}\cup\{0\}\bigr).
$$

The last selected box before $j$, if any, supplies exactly one of these candidates; conversely an optimal candidate subsequence can be extended by $j$. [Induction](../../../../../../mathematical-induction.md) on $j$ proves the [box nesting](../../../../../../box-nesting.md) recurrence. Store a maximizing predecessor index and reconstruct from an index maximizing $F[j]$. For $n=0$, return the empty subsequence.

There are $O(n^2)$ candidate pairs, each requiring $O(d)$ coordinate comparisons. Hence **$O(nd\log d+n^2d)$ [running time](../../../../../../running-time.md) and $O(nd+n)$ storage** suffice, including sorted vectors, table entries and reconstruction pointers. It is unnecessary to store every fitting pair.

If “subsequence” was intended to allow arbitrary reordering, build the containment [Directed acyclic graph](../../../../../../directed-acyclic-graph.md) instead: include every fitting ordered pair, then find its longest chain. Strict increase of the smallest sorted dimension gives a [topological sorting](../../../../../../topological-sorting.md) by that dimension. The same pair-testing bound applies, but the index restriction must then be removed. These two interpretations differ: input boxes $(3,3),(2,2)$ have a longest order-preserving subsequence of one box, but an unrestricted nesting chain of two.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [8](../../../8.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
