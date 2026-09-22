<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use these [structural recursion](../../../../../structural-recursion.md) definitions in [Haskell](../../../../../haskell.md):
```
tails :: [a] -> [[a]]
tails xs = xs : ptails xs

ptails :: [a] -> [[a]]
ptails [] = []
ptails (_:xs) = tails xs

ntails :: [a] -> [[a]]
ntails [] = []
ntails xs@(_:rest) = xs : ntails rest
```
The first definition returns a known outer constructor even when `xs` is undefined, so `null (tails undefined)` is `False`, as required. The pattern in `ntails` must first determine whether the input is empty. Each [suffix of a list](../../../../../suffix-of-a-list.md) is shared with the original [list](../../../../../list-abstract-data-type.md); on a finite input of length $n$, constructing the outer lists takes $O(n)$ work and additional outer-list space. No suffix is copied or measured repeatedly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
