<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The necessary domain is a finite, nonempty [list](../../../../../list-abstract-data-type.md): the datatype has no representation of an empty leaf sequence, and the supplied size-based balance condition does not specify an infinite-size construction.

```
build :: [a] -> Tree a
build []  = error "build: empty input"
build [x] = One x
build xs  = Two (build ys) (build zs)
  where
    (ys,zs) = split (length xs `div` 2) xs
```

For length $n\ge2$, the two nonempty pieces have $\lfloor n/2\rfloor$ and $\lceil n/2\rceil$ elements. Their sizes differ by at most one, and both are shorter than the input. [Induction](../../../../../mathematical-induction.md) therefore proves termination and the required [leaf-balanced binary tree](../../../../../leaf-balanced-binary-tree.md) property at every node. The same [induction](../../../../../mathematical-induction.md), using `ys ++ zs = xs`, proves `flatten (build xs) = xs`. This straightforward implementation takes $O(n\log n)$ [running time](../../../../../running-time.md); computing the length repeatedly is acceptable here because no faster construction was requested.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
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
