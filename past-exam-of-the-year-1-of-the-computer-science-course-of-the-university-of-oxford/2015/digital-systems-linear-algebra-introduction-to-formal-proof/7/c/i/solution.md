<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extract both [negations](../../../../../../negation.md), assume the [logical disjunction](../../../../../../logical-disjunction.md), and use [disjunction elimination](../../../../../../disjunction-elimination-rule.md) to derive [logical falsity](../../../../../../logical-falsity.md) in either case:

$$
\begin{array}{rll}
1&\neg P\land\neg Q&\text{premise}\\
2&\neg P&\land\text{-elim-L }1\\
3&\neg Q&\land\text{-elim-R }1\\
4&\vert\ P\lor Q&\text{assumption}\\
5&\vert\ \vert\ P&\text{first case assumption}\\
6&\vert\ \vert\ \bot&\neg\text{-elim }5,2\\
7&\vert\ \vert\ Q&\text{second case assumption}\\
8&\vert\ \vert\ \bot&\neg\text{-elim }7,3\\
9&\vert\ \bot&\lor\text{-elim }4,5\text{--}6,7\text{--}8\\
10&\neg(P\lor Q)&\neg\text{-intro }4\text{--}9
\end{array}
$$

The two case [subproofs](../../../../../../subproof.md) are siblings, not nested within one another. Therefore

$$
\boxed{\neg P\land\neg Q\ \vdash\ \neg(P\lor Q).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
