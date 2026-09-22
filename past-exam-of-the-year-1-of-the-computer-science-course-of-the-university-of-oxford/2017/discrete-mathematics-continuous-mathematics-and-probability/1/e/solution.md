<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the convention that $R\circ S$ applies $S$ first. Reflexivity inserts an identity step: if $aRb$, use $aSa$ to obtain $(a,b)\in R\circ S$; if $aSb$, use $bRb$ for the same conclusion. Thus $R\cup S\subseteq R\circ S$. By [monotonicity of relation composition](../../../../../monotonicity-of-relation-composition.md),

$$
(R\cup S)\circ(R\cup S)\subseteq(R\circ S)\circ(R\circ S).
$$

For strictness, take $A=\{0,1,2,3\}$ and let $R=S$ consist of the identity pairs together with $(0,1),(1,2),(2,3)$. Both are [reflexive relations](../../../../../reflexive-relation.md). The left side permits at most two forward chain steps, so does not contain $(0,3)$. The right side permits four steps, including $0\to1\to2\to3\to3$, so does contain it. Equality therefore need not hold.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
