<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Haskell](../../../../../haskell.md) [type signatures](../../../../../type-signature.md) are **`take :: Int -> [a] -> [a]` and `drop :: Int -> [a] -> [a]`**. These definitions also handle nonpositive counts as the Prelude does:
```
take n _ | n <= 0 = []
take _ [] = []
take n (x:xs) = x : take (n-1) xs

drop n xs | n <= 0 = xs
drop _ [] = []
drop n (_:xs) = drop (n-1) xs
```
The wildcard in the first equation matters under [lazy evaluation](../../../../../lazy-evaluation.md): `take 0 undefined` yields `[]` without inspecting its [list](../../../../../list-abstract-data-type.md) argument. The remainder of this question uses nonnegative counts.[§9, Standard Prelude, definitions and types of take and drop](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
