<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite even [lists](../../../../../list-abstract-data-type.md), these definitions take at most [linear time](../../../../../linear-time.md):
```
halve :: [a] -> ([a],[a])
halve xs = splitAt (length xs `div` 2) xs

pairs :: [a] -> [(a,a)]
pairs [] = []
pairs (x:y:xs) = (x,y) : pairs xs
pairs [_] = error "pairs: odd length"
```
The length calculation and the prefix split each take $O(n)$ time. The second operation consumes two constructors per step and emits one pair. Under the stated even-length precondition, neither definition encounters an unmatched final element.

## ↑ Ancestors (12)

1. [A](../a.md)
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
