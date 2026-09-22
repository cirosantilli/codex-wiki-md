<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First obtain $A$ by a [double-negation elimination](../../../../../../double-negation-elimination.md), then obtain $\neg B$ by the [negation introduction rule](../../../../../../negation-introduction-rule.md). The following [natural deduction](../../../../../../natural-deduction.md) proof uses only the printed rules, with $\bot E$ denoting the [logical falsity elimination rule](../../../../../../logical-falsity-elimination-rule.md):

$$
\begin{array}{rll}
1&\neg(A\to B)&\text{premise}\\
2&[\neg A]^a&\text{assumption}\\
3&\quad[A]^b&\text{assumption}\\
4&\qquad\bot&\neg E\ 3,2\\
5&\qquad B&\bot E\ 4\\
6&\quad A\to B&\to I\ (3\text{--}5)\\
7&\quad\bot&\neg E\ 6,1\\
8&\neg\neg A&\neg I\ (2\text{--}7)\\
9&A&\neg\neg E\ 8\\
10&[B]^c&\text{assumption}\\
11&\quad[A]^d&\text{assumption}\\
12&\qquad B&\text{reiteration of 10}\\
13&\quad A\to B&\to I\ (11\text{--}12)\\
14&\quad\bot&\neg E\ 13,1\\
15&\neg B&\neg I\ (10\text{--}14)\\
16&A\land\neg B&\land I\ 9,15.
\end{array}
$$

Reiteration only reuses an available line within its scope. In particular, the unused [temporary assumption](../../../../../../temporary-assumption.md) on line 11 is legitimately discharged by the [implication introduction rule](../../../../../../implication-introduction-rule.md).

$$
\boxed{\neg(A\to B)\vdash A\land\neg B.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
