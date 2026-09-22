<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A shared [recursion](../../../../../recursion-computer-science.md) computes both components:

```
split :: Int -> [a] -> ([a],[a])
split n xs | n <= 0 = ([],xs)
split _ []         = ([],[])
split n (x:xs)     = (x:ys,zs)
  where (ys,zs) = split (n-1) xs
```

For a defined count and a spine with $m$ available constructors before termination, each of `take` and `drop` makes $\min(\max(n,0),m)$ recursive calls, whereas `split` makes that many once. **The number of recursive calls is halved.** The [irrefutable pattern](../../../../../irrefutable-pattern.md) in the local pair binding also avoids evaluating the recursive pair merely to expose the first output element.

On [proper lazy lists](../../../../../proper-lazy-list.md) this has the intended two component values. There is a small [bottom value](../../../../../bottom-value.md) distinction outside that domain: the displayed single-pass definition must inspect a positive-count input spine before returning its outer pair, whereas the literal expression `(take n xs, drop n xs)` exposes the pair constructor even if `xs` is undefined. The algorithmic answer concerns the two components and the stated call count; it need not silently claim equality under a test that observes this outer constructor alone.

## ↑ Ancestors (12)

1. [B](../b.md)
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
