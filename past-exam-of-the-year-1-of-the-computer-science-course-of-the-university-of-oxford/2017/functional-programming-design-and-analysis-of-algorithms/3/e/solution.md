<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Prune until a [fixed point](../../../../../fixed-point.md) before enumerating the surviving domains:

```
stable :: Eq a => (a -> a) -> a -> a
stable f x = let y = f x
             in if y == x then x else stable f y

solve :: Grid -> [Grid]
solve = filter complete . expand . stable prune . choices
```

New singleton cells can make a later pruning pass effective even if one pass has already run. Under the supplied deletion-only, solution-preserving contract, [fixed-point pruning of finite constraint domains](../../../../../fixed-point-pruning-of-finite-constraint-domains.md) terminates: every changed pass strictly decreases the total number of candidates, initially at most $81\cdot9=729$. No valid solution is removed. An empty domain causes `expand` to return no candidates; a fixed point with unresolved alternatives still needs enumeration and the final `complete` test.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
