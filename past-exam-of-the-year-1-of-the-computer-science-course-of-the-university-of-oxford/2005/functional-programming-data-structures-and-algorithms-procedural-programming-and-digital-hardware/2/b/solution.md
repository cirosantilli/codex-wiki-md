<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [permutation generation by insertion](../../../../../permutation-generation-by-insertion.md): recursively arrange the tail, then insert the removed head in every possible position.

```
inserts x [] = [[x]]
inserts x (y:ys) = (x:y:ys) : map (y:) (inserts x ys)

perms [] = [[]]
perms (x:xs) = concat (map (inserts x) (perms xs))
```

The [map function](../../../../../map-higher-order-function.md) in `inserts` prefixes `y` to each placement after the first position. For a [list](../../../../../list-abstract-data-type.md) of length $k$, the number of results obeys $I(0)=1$ and $I(k+1)=1+I(k)$, so [mathematical induction](../../../../../mathematical-induction.md) gives $I(k)=k+1$. Every result still contains the same $k$ old elements and the one inserted element.

Let $P(n)$ be the length of `perms xs` for an input of length $n$. There is exactly one [permutation](../../../../../permutation.md) of the empty [list](../../../../../list-abstract-data-type.md), namely the empty [list](../../../../../list-abstract-data-type.md) itself: hence `perms []` is `[[]]`, with length one. For a nonempty input, each recursively obtained [permutation](../../../../../permutation.md) has length $n-1$ and gives $n$ placements. Thus

$$
P(0)=1=0!,\qquad P(n)=nP(n-1),\qquad
\boxed{P(n)=n!.}
$$

Length alone would not exclude repeated answers. Since the input elements are distinct, removing the distinguished element $x$ from any result uniquely recovers both its placement and the shorter [permutation](../../../../../permutation.md). Hence different construction choices give different outputs, and every desired [permutation](../../../../../permutation.md) is obtained by inserting $x$ into its restriction to `xs`. For `[a,b,c]`, this code yields `[a,b,c]`, `[b,a,c]`, `[b,c,a]`, `[a,c,b]`, `[c,a,b]`, `[c,b,a]`, each exactly once.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
