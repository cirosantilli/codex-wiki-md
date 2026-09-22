<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Generate successive states lazily and take exactly their initial nonempty segment:
```
runSystem :: (State, [Rule]) -> [State]
runSystem (state, rules) =
  takeWhile (not . null) (iterate (step rules) state)
```
The [iterate function](../../../../../haskell-iterate-function.md) starts with `state` itself and repeatedly applies `step rules`. The [takeWhile function](../../../../../haskell-takewhile-function.md) excludes the first empty state and everything after it. If the initial state is empty, the result is `[]`. If the process never reaches an empty state, the answer is a potentially infinite [list](../../../../../list-abstract-data-type.md) whose finite prefixes can be observed through [lazy evaluation](../../../../../lazy-evaluation.md). No artificial maximum number of rewriting steps is introduced.

## ↑ Ancestors (12)

1. [C](../c.md)
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
