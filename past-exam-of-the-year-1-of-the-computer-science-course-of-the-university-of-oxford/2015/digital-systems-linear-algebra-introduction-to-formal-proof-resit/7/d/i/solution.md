<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $F=(\neg P)\to Q$ and $G=(\neg P)\to\neg Q$. Use the printed [implication elimination rule](../../../../../../implication-elimination-rule.md), [negation elimination rule](../../../../../../negation-elimination-rule.md), [negation introduction rule](../../../../../../negation-introduction-rule.md), [double-negation elimination](../../../../../../double-negation-elimination.md) and [implication introduction rule](../../../../../../implication-introduction-rule.md):

$$
\begin{array}{rll}
1&F&\text{premise}\\
2&[F]^a&\text{assumption}\\
3&\quad[G]^b&\text{assumption}\\
4&\qquad[\neg P]^c&\text{assumption}\\
5&\qquad\quad Q&\to E\ 4,2\\
6&\qquad\quad\neg Q&\to E\ 4,3\\
7&\qquad\quad\bot&\neg E\ 5,6\\
8&\qquad\neg\neg P&\neg I\ (4\text{--}7)\\
9&\qquad P&\neg\neg E\ 8\\
10&\quad G\to P&\to I\ (3\text{--}9)\\
11&F\to(G\to P)&\to I\ (2\text{--}10).
\end{array}
$$

Line 1 is the given premise; the argument actually establishes the conclusion without needing it, since line 2 supplies its own copy of $F$. Introducing and discharging this separate [temporary assumption](../../../../../../temporary-assumption.md) preserves the exact printed conclusion.

$$
\boxed{(\neg P)\to Q\ \vdash\ ((\neg P)\to Q)\to(((\neg P)\to\neg Q)\to P).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
