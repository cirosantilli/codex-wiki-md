<h1 id="6/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $C$ be the final `A` [set](../../../../../../set-split.md) produced by the [algorithm](../../../../../../algorithm-split.md). It contains the initial `A` set, and every [vertex](../../../../../../vertex-graph-theory.md) outside $C$ has at most half its neighbours in $C$: otherwise its final key would still be positive. Thus $C$ is closed under the activation rule.

Now consider _any_ legal sequence, including sequences which change some `A` preferences back to `B`. We prove by [induction](../../../../../../mathematical-induction.md) that its current `A` set is always a [subset](../../../../../../subset.md) of $C$. This is true initially. A switch to `B` preserves the inclusion. If a [vertex](../../../../../../vertex-graph-theory.md) outside $C$ were to switch to `A`, its `A` neighbours would all lie in $C$, so their number could not exceed half its degree. Such a switch is forbidden. A switch inside $C$ also preserves the inclusion.

Consequently every attainable final `A` set has size at most $|C|$. The [algorithm](../../../../../../algorithm-split.md) supplies a legal sequence attaining $C$ itself, so **its sequence is optimal**. This [closure dominance for asynchronous threshold switching](../../../../../../closure-dominance-for-asynchronous-threshold-switching.md) proves more than a local-greedy claim: temporary losses of `A` [vertices](../../../../../../vertex-graph-theory.md) cannot unlock an additional [vertex](../../../../../../vertex-graph-theory.md) outside the activation closure.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
