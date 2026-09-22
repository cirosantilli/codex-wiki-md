<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**In general, no direct [list fold](../../../../../list-fold.md) with result type `[a]` can implement `dropWhile p`.** Choose total values $u,v$ for which $p(u)=\mathrm{True}$ and $p(v)=\mathrm{False}$. The results on `[]` and `[u]` are both `[]`. A hypothetical implementation `foldr h z` would therefore receive identical folded-tail values when extending either input by the same head $v$. Yet the required outputs are `[v]` and `[v,u]`, respectively. This contradicts the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md): the combining [function](../../../../../function-split.md) cannot distinguish information already discarded by its tail summary.

The claim concerns a direct same-result-type [list fold](../../../../../list-fold.md). A [list fold](../../../../../list-fold.md) returning extra information, followed by a projection, is possible: a pair can retain both the original tail and the dropped [list suffix](../../../../../suffix-of-a-list.md). Also, special [predicates](../../../../../predicate.md) can have direct [list folds](../../../../../list-fold.md): a constantly false [predicate](../../../../../predicate.md) gives the identity; a constantly true [predicate](../../../../../predicate.md) can use `foldr (\_ r -> r) []`, which correctly diverges when it must traverse an infinite spine. Those special cases do not supply an implementation for an arbitrary [predicate](../../../../../predicate.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
