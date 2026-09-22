<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A call can instead produce an entire run and recurse on the unused input:
```
groupRuns :: Eq a => [a] -> [[a]]
groupRuns [] = []
groupRuns (x:xs) = (x:ys) : groupRuns zs
  where (ys,zs) = span (== x) xs
```
Here `span` returns the longest matching [prefix of a list](../../../../../prefix-of-a-list.md) and the remaining [suffix of a list](../../../../../suffix-of-a-list.md). Thus `x:ys` is the first maximal run, while `zs` begins the next run or is empty. Each recursive call produces one outer output element. The lazy pair binding permits output of the first constructor before the run's endpoint is known. Every finite input position is scanned a bounded number of times, so the [time complexity](../../../../../time-complexity.md) is $\Theta(n)$ for unit-cost equality, including output construction.[Chapter 9, Standard Prelude, definition of span](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
