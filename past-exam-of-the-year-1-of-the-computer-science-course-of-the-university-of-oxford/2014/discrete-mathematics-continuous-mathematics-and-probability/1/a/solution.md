<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [De Morgan's laws](../../../../../de-morgan-s-laws.md), taking a [set difference](../../../../../set-difference.md) from a [union](../../../../../set-union.md) requires exclusion from both [sets](../../../../../set-split.md), while taking a [set difference](../../../../../set-difference.md) from an [intersection](../../../../../set-intersection.md) requires exclusion from at least one:

$$
\boxed{A\setminus(B\cup C)=(A\setminus B)\cap(A\setminus C),\qquad A\setminus(B\cap C)=(A\setminus B)\cup(A\setminus C).}
$$

For example, $x$ belongs to the first left-hand side precisely when $x\in A$, $x\notin B$ and $x\notin C$; these are exactly the membership conditions on the first right-hand side. For the second identity, replace the two exclusions by their [logical disjunction](../../../../../logical-disjunction.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
