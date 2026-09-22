<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Keep the premise $P\to Q$ open. Assume $Q\to\neg P$, then temporarily assume $P$. Two applications of the [implication elimination rule](../../../../../implication-elimination-rule.md) produce $Q$ and then $\neg P$, contradicting the temporary $P$. Discharge $P$ using the [negation introduction rule](../../../../../negation-introduction-rule.md), then discharge $Q\to\neg P$ using the [implication introduction rule](../../../../../implication-introduction-rule.md).

$$
\begin{array}{rll}
1.&P\to Q&\text{premise}\\
2.&\quad Q\to\neg P&\text{assumption }[i]\\
3.&\qquad P&\text{assumption }[j]\\
4.&\qquad Q&\to\text{-elimination, }1,3\\
5.&\qquad\neg P&\to\text{-elimination, }2,4\\
6.&\qquad\bot&\neg\text{-elimination, }3,5\\
7.&\quad\neg P&\neg\text{-introduction, }3\text{--}6;\ [j]\text{ discharged}\\
8.&(Q\to\neg P)\to\neg P&\to\text{-introduction, }2\text{--}7;\ [i]\text{ discharged}.
\end{array}
$$

This [natural deduction](../../../../../natural-deduction.md) proof uses only the supplied introduction and elimination rules. Line 6 is an application of the [negation elimination rule](../../../../../negation-elimination-rule.md); no classical contradiction principle is needed.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [7](../../7.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
