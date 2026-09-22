<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every accumulator $a$, [pattern matching](../../../../../pattern-matching.md) makes `foldl s a undefined` the [bottom value](../../../../../bottom-value.md). Now use [structural induction](../../../../../structural-induction.md) on a finite [list prefix](../../../../../prefix-of-a-list.md) ending in the [bottom value](../../../../../bottom-value.md). The induction step is `foldl s a (x:ps) = foldl s (s a x) ps`; the induction hypothesis applies to _every_ accumulator, including `s a x`. Consequently every such finite approximation has result $\bot$.

An infinite [lazy list](../../../../../lazy-list.md) is the limit of its finite prefixes, each interpreted as a [finite approximation of a lazy list](../../../../../finite-approximation-of-a-lazy-list.md). Definable [Haskell](../../../../../haskell.md) operations are [Scott continuous maps](../../../../../scott-continuity.md), so the result on the infinite [lazy list](../../../../../lazy-list.md) is the supremum of the results on these approximations. Every result is $\bot$, hence **`foldl s a xs = undefined` on every infinite input spine**, irrespective of whether `s` would inspect the accumulator.

For a concrete separation, choose `s = (&&)`, `a = True`, and `xs = False : repeat True`. The [left fold](../../../../../left-fold.md) is $\bot$, whereas the [right fold](../../../../../list-fold.md) returns **`False`** after observing the first element: `False && r` does not demand `r`. It is reaching the end of the input spine, rather than strictness of the combining operation, that prevents this [left fold](../../../../../left-fold.md) from returning.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
