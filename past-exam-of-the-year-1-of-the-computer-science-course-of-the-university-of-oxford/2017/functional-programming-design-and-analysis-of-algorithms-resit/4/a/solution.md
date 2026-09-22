<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The most general [polymorphic type](../../../../../polymorphic-type.md) is

```
unfold :: (s -> Bool) -> (s -> a) -> (s -> s) -> s -> [a]
```

The stopping [predicate](../../../../../predicate.md) consumes a state, the output function turns that state into one list element, and the transition function supplies another state of the same type. The state type and output type need not coincide. This is a [list unfold](../../../../../list-unfold.md) with separate stopping, output and transition arguments.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
