<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Generate the successive states using the [Haskell iterate function](../../../../../haskell-iterate-function.md), keep those before the stopping test becomes true using the [Haskell takeWhile function](../../../../../haskell-takewhile-function.md), then map the output function:

```
unfoldU :: (s -> Bool) -> (s -> a) -> (s -> s) -> s -> [a]
unfoldU p f g = map f . takeWhile (not . p) . iterate g
```

The missing expression is therefore $\boxed{\operatorname{takeWhile}(\operatorname{not}\circ p)\circ\operatorname{iterate}(g)}$. On states $x,g(x),g^2(x),\ldots$, the first state satisfying `p` is excluded, just as in the recursive [list unfold](../../../../../list-unfold.md). If no state satisfies `p`, the result is an infinite [lazy list](../../../../../lazy-list.md), provided each demanded test, output and transition terminates.

## ↑ Ancestors (12)

1. [B](../b.md)
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
