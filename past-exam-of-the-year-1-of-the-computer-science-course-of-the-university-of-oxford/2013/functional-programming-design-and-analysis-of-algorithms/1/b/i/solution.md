<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the [type signature](../../../../../../type-signature.md) `map :: (u -> v) -> [u] -> [v]`, the supplied [function](../../../../../../function-split.md) is `concat :: [[a]] -> [a]`. [Type inference](../../../../../../type-inference.md) therefore identifies `u` with `[[a]]` and `v` with `[a]`. Consequently,

```
map concat :: [[[a]]] -> [[a]]
```

Thus $\boxed{[[[\alpha]]]\to[[\alpha]]}$ is the [principal type](../../../../../../principal-type.md). For example, `map concat [[[1],[2,3]],[[4],[]]]` gives `[[1,2,3],[4]]`: it concatenates each inner group, preserving the outermost grouping.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
