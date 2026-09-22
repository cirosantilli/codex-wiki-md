<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite [lists](../../../../../list-abstract-data-type.md), use [structural induction](../../../../../structural-induction.md): establish `P []`; then, for arbitrary `x` and `xs`, assume `P xs` and prove `P (x:xs)`. The [induction hypothesis](../../../../../induction-hypothesis.md) must quantify over any other parameters that need to change in the step.

For _all_ [Haskell](../../../../../haskell.md) [list](../../../../../list-abstract-data-type.md) values, finite terminating spines are insufficient: also establish `P undefined`, and allow arbitrary, possibly undefined, heads in the cons step. This proves the equation for finite [partial lists](../../../../../partial-list.md) ending in the [bottom value](../../../../../bottom-value.md). An infinite [lazy list](../../../../../lazy-list.md) is the limit of these finite approximations. Equations between pure definable [computable functions](../../../../../computable-function.md) are preserved by those limits, so the equation extends to infinite inputs. This last argument requires that admissibility property; an arbitrary logical property of [lists](../../../../../list-abstract-data-type.md) need not have it. The distinction between `[]` and the [bottom value](../../../../../bottom-value.md) is essential.[§3.1, Errors, and §3.17.2, Informal Semantics of Pattern Matching](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
