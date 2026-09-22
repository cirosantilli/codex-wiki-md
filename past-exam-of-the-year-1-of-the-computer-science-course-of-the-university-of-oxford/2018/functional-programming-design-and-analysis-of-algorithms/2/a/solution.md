<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual left-to-right [pattern matching](../../../../../pattern-matching.md) order:

```
zip :: [a] -> [b] -> [(a,b)]
zip []     _      = []
zip _      []     = []
zip (x:xs) (y:ys) = (x,y) : zip xs ys
```

The result stops when either [list](../../../../../list-abstract-data-type.md) ends, so its length on finite total inputs is the smaller input length. Elements remaining in the longer [list](../../../../../list-abstract-data-type.md) are discarded.

Strictness is asymmetric. Writing the [bottom value](../../../../../bottom-value.md) as $\bot$, **`zip` is strict in its first list but not uniformly strict in its second**: `zip undefined ys` is undefined, whereas `zip [] undefined = []`. With a nonempty first [list](../../../../../list-abstract-data-type.md), an undefined second [list](../../../../../list-abstract-data-type.md) does make the result undefined. Neither pair component is forced merely to produce the outer result constructor: `zip [undefined] [undefined]` already has a defined outer cons and pair. This follows from ordered [pattern matching](../../../../../pattern-matching.md) and [lazy evaluation](../../../../../lazy-evaluation.md), not from the behavior on total [lists](../../../../../list-abstract-data-type.md) alone.[§3.17.2, ordered pattern matching; Chapter 9, zip in the Standard Prelude](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
