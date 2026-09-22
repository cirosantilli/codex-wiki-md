<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Read chained [logical implications](../../../../../../logical-implication.md) as right-associative. Use the following [natural deduction](../../../../../../natural-deduction.md) derivation; indentation bars mark nested [subproofs](../../../../../../subproof.md) and the last column records rules and discharged line ranges:

$$
\begin{array}{rll}
1&E\to(F\to(G\to H))&\text{premise}\\
2&\vert\ G&\text{assumption}\\
3&\vert\ \vert\ F&\text{assumption}\\
4&\vert\ \vert\ \vert\ E&\text{assumption}\\
5&\vert\ \vert\ \vert\ F\to(G\to H)&\to\text{-elim }1,4\\
6&\vert\ \vert\ \vert\ G\to H&\to\text{-elim }5,3\\
7&\vert\ \vert\ \vert\ H&\to\text{-elim }6,2\\
8&\vert\ \vert\ E\to H&\to\text{-intro }4\text{--}7\\
9&\vert\ F\to(E\to H)&\to\text{-intro }3\text{--}8\\
10&G\to(F\to(E\to H))&\to\text{-intro }2\text{--}9
\end{array}
$$

Each application of the [implication introduction rule](../../../../../../implication-introduction-rule.md) discharges only its matching [temporary assumption](../../../../../../temporary-assumption.md). Thus

$$
\boxed{E\to F\to G\to H\ \vdash\ G\to F\to E\to H.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
