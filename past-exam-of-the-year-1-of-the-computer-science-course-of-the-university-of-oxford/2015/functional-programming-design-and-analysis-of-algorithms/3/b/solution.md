<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply one replacement to each original character and concatenate the results:
```
step :: [Rule] -> State -> State
step rules = concatMap (applyRule rules)
```
The [concatMap](../../../../../haskell-concatmap-function.md) operation combines a [map function](../../../../../map-higher-order-function.md) and [list concatenation](../../../../../list-concatenation.md). Replacements occur in original-character order, so a character produced by a replacement is not processed again during the same step. This is parallel [string rewriting](../../../../../string-rewriting.md). In particular `step rules "" = ""`, with no rule lookup required for the empty state.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
