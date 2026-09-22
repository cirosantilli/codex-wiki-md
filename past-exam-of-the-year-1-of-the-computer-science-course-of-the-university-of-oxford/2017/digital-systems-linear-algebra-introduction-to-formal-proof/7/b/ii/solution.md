<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the negation of the desired disjunction, derive both negated propositions and contradict the premise. The [natural deduction](../../../../../../natural-deduction.md) derivation is

$$
\begin{array}{rll}
1&\neg(\neg P\land\neg Q)&\text{premise}\\
2&\quad\neg(P\lor Q)&\text{assumption}\\
3&\qquad P&\text{assumption}\\
4&\qquad P\lor Q&\lor I\ 3\\
5&\qquad\bot&\neg E\ 4,2\\
6&\quad\neg P&\neg I\ 3\text{--}5\\
7&\qquad Q&\text{assumption}\\
8&\qquad P\lor Q&\lor I\ 7\\
9&\qquad\bot&\neg E\ 8,2\\
10&\quad\neg Q&\neg I\ 7\text{--}9\\
11&\quad\neg P\land\neg Q&\land I\ 6,10\\
12&\quad\bot&\neg E\ 11,1\\
13&P\lor Q&\mathrm{RAA}\ 2\text{--}12
\end{array}
$$

The proof uses [disjunction introduction](../../../../../../disjunction-introduction-rule.md), [conjunction introduction](../../../../../../conjunction-introduction-rule.md) and the classical RAA rule; it does not silently replace the required derivation by a truth-table check.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
