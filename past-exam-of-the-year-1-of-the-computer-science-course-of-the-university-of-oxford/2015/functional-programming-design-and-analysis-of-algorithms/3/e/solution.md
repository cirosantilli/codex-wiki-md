<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Attach zero-based indices before filtering:
```
findStates :: [State] -> String -> [(State, Integer)]
findStates states str =
  [(state, i) |
     (state, i) <- zip states [0..],
     isPrefix str state]
```
The [zip function](../../../../../haskell-zip-function.md) pairs each state with its position in the original sequence. The [list comprehension](../../../../../list-comprehension.md) retains exactly those pairs satisfying the [prefix](../../../../../prefix-of-a-list.md) test, preserving their order and their original indices. The declared result makes `[0..]` a stream of `Integer` indices. An empty search string matches every state, including an empty state, because the empty [list](../../../../../list-abstract-data-type.md) is a [prefix](../../../../../prefix-of-a-list.md) of every [list](../../../../../list-abstract-data-type.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
