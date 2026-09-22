<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Flatten the days, emit both participants of every match and remove repeated names:

```
teams :: [[Match]] -> [Team]
teams days = unique [t | Match a _ b _ <- concat days, t <- [a,b]]
  where
    unique []     = []
    unique (t:ts) = t : unique (filter (/= t) ts)
```

Every emitted name belongs to some match, and every participating team enters the intermediate [list](../../../../../list-abstract-data-type.md). At each recursive step, `unique` emits its first remaining name once and deletes precisely its later occurrences. [Induction](../../../../../mathematical-induction.md) therefore proves both coverage and absence of duplicates. The output preserves first appearance; no particular team ordering was required. This simple [list](../../../../../list-abstract-data-type.md) implementation can take quadratic time in the number of participant occurrences, which is permissible here; the question imposes no efficiency target.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
