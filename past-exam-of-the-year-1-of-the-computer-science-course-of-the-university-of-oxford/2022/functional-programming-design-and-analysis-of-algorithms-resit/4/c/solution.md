<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interleave equal halves, or collect the first and second components of adjacent pairs:
```
riffle :: [a] -> [a]
riffle = unpairs . uncurry zip . halve

unriffle :: [a] -> [a]
unriffle = unhalve . unzip . pairs
```
For halves `as` and `bs` of equal length, `pairs (riffle xs) = zip as bs`, and `unzip (zip as bs) = (as,bs)`. Therefore `unriffle (riffle xs) = xs`. Conversely, starting from the adjacent pairs of any even [list](../../../../../list-abstract-data-type.md), separating the components, halving their concatenation and zipping them restores those same pairs. Hence `riffle (unriffle xs) = xs` too. Every stage takes [linear time](../../../../../linear-time.md). This [perfect out-shuffle](../../../../../perfect-out-shuffle.md) leaves the first and last positions fixed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
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
