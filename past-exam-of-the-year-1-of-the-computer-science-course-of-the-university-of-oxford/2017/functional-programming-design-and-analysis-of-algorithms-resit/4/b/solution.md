<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The standard [Haskell](../../../../../haskell.md) definition and principal type are

```
iterate :: (a -> a) -> a -> [a]
iterate f x = x : iterate f (f x)
```

Under [lazy evaluation](../../../../../lazy-evaluation.md), this produces successive states $x,f(x),f(f(x)),\ldots$ as demanded. An infinite spine does not require all elements to be evaluated at once; [productivity](../../../../../stream-productivity.md) still depends on the demanded computations terminating.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
