<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Include nonpositive counts and exhausted input explicitly:

```
take :: Int -> [a] -> [a]
take n _      | n <= 0 = []
take _ []             = []
take n (x:xs)         = x : take (n-1) xs

drop :: Int -> [a] -> [a]
drop n xs     | n <= 0 = xs
drop _ []             = []
drop n (_:xs)         = drop (n-1) xs
```

The tests on the count precede inspection of the input [list](../../../../../list-abstract-data-type.md). Thus `take 0 undefined = []`, while `drop 0 undefined = undefined`, exactly as these [list prefix](../../../../../prefix-of-a-list.md) and [list suffix](../../../../../suffix-of-a-list.md) operations require. No element value is inspected merely to traverse the spine.[Chapter 9, PreludeList: take and drop](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
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
