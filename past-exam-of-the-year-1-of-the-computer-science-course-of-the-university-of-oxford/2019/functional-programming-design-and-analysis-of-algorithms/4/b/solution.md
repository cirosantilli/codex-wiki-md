<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Swap roles after emitting one element:

```
interleave :: [a] -> [a] -> [a]
interleave []     ys = ys
interleave (x:xs) ys = x : interleave ys xs
```

While both [lists](../../../../../list-abstract-data-type.md) are nonempty, the [function](../../../../../function-split.md) alternates between them. Their $j$-th input occurrences appear after at most $2j+2$ output steps, counting positions from zero; once either [list](../../../../../list-abstract-data-type.md) ends, the other is returned directly. Every output constructor comes from one input constructor, and every input occurrence is eventually selected. This proves [fair enumeration](../../../../../fair-enumeration.md) and [productivity](../../../../../stream-productivity.md) on the two [proper lazy lists](../../../../../proper-lazy-list.md), including two infinite ones.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
