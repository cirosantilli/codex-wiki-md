<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The test consumes a state and returns `Bool`; the output function maps a state to an element; and the transition preserves the state type. Hence the most general [polymorphic](../../../../../programming-language-polymorphism.md) [type signature](../../../../../type-signature.md) is

```
unfold :: (s -> Bool) -> (s -> a) -> (s -> s) -> s -> [a]
```

Equivalently, $\boxed{(\sigma\to\mathrm{Bool})\to(\sigma\to\alpha)\to(\sigma\to\sigma)\to\sigma\to[\alpha]}$. The state and emitted element can have unrelated types. A [list unfold](../../../../../list-unfold.md) produces the next element from the current state, then advances to a new state.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
