<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [negation introduction](../../../../../../negation-introduction-rule.md) separately for each component, introducing the forbidden [logical disjunction](../../../../../../logical-disjunction.md) in each [subproof](../../../../../../subproof.md):

$$
\begin{array}{rll}
1&\neg(P\lor Q)&\text{premise}\\
2&\vert\ P&\text{assumption}\\
3&\vert\ P\lor Q&\lor\text{-intro-L }2\\
4&\vert\ \bot&\neg\text{-elim }3,1\\
5&\neg P&\neg\text{-intro }2\text{--}4\\
6&\vert\ Q&\text{assumption}\\
7&\vert\ P\lor Q&\lor\text{-intro-R }6\\
8&\vert\ \bot&\neg\text{-elim }7,1\\
9&\neg Q&\neg\text{-intro }6\text{--}8\\
10&\neg P\land\neg Q&\land\text{-intro }5,9
\end{array}
$$

Both [temporary assumptions](../../../../../../temporary-assumption.md) have been discharged before the final [conjunction introduction](../../../../../../conjunction-introduction-rule.md), so

$$
\boxed{\neg(P\lor Q)\ \vdash\ \neg P\land\neg Q.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
