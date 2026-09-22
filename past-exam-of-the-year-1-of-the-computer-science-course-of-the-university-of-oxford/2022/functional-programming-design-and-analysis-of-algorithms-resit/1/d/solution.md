<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a type with distinct values `a` and `n`, and let `s _ y = y`. Suppose a direct [right fold](../../../../../list-fold.md) with the same result type represented this [left fold](../../../../../left-fold.md). The empty [list](../../../../../list-abstract-data-type.md) forces `k = n`. The singleton [lists](../../../../../list-abstract-data-type.md) force `c n n = n` and `c a n = a`. But then
```
foldr c k [a,n] = c a (c n n) = c a n = a,
foldl s n [a,n] = n.
```
Since `a /= n`, this is a [counterexample](../../../../../counterexample.md). A direct [right fold](../../../../../list-fold.md) cannot recover whether its tail result `n` came from the empty [list](../../../../../list-abstract-data-type.md) or from the singleton `[n]`. The obstruction already occurs on finite total inputs, so it also rules out an implementation valid on all [lazy lists](../../../../../lazy-list.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
