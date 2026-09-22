<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Simultaneous [propositional substitution](../../../../../propositional-substitution.md) gives

$$
\varphi S=((X\land Y)\to\neg(X\lor Y))\lor(\neg Y\land\neg(X\land Y)).
$$

Let $K=\neg(X\land Y)$. The first disjunct equals $K\lor\neg(X\lor Y)$. By [De Morgan's laws](../../../../../de-morgan-s-laws.md), $\neg(X\lor Y)=\neg X\land\neg Y$ implies $K=\neg X\lor\neg Y$, so absorption reduces that first disjunct to $K$. The second disjunct is $\neg Y\land K$ and is also absorbed by $K$. Therefore

$$
\boxed{\varphi S\equiv\neg(X\land Y)\equiv\neg X\lor\neg Y.}
$$

The resulting [Boolean function](../../../../../boolean-function.md) is false only when both $X$ and $Y$ are true, providing a four-row [truth table](../../../../../truth-table.md) check.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
