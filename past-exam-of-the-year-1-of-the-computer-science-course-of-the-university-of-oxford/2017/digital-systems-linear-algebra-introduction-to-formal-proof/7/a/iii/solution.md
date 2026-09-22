<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $H=\neg(P\to\neg Q)$. First derive $Q$, then $P$, using the derived [proof by contradiction](../../../../../../reductio-ad-absurdum.md) rule. Indentation records the [subproofs](../../../../../../subproof.md):

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&\quad\neg Q&\text{assumption}\\
3&\qquad P&\text{assumption}\\
4&\qquad\neg Q&\text{reiterate }2\\
5&\quad P\to\neg Q&\to I\ 3\text{--}4\\
6&\quad\bot&\neg E\ 1,5\\
7&Q&\mathrm{RAA}\ 2\text{--}6\\
8&\quad\neg P&\text{assumption}\\
9&\qquad P&\text{assumption}\\
10&\qquad\bot&\neg E\ 9,8\\
11&\qquad\neg Q&\bot E\ 10\\
12&\quad P\to\neg Q&\to I\ 9\text{--}11\\
13&\quad\bot&\neg E\ 1,12\\
14&P&\mathrm{RAA}\ 8\text{--}13\\
15&Q\land P&\land I\ 7,14
\end{array}
$$

Line 11 uses [explosion](../../../../../../logical-falsity-elimination-rule.md); lines 5 and 12 discharge only their inner assumptions. Each RAA step can be expanded into [negation introduction](../../../../../../negation-introduction-rule.md) followed by [double-negation elimination](../../../../../../double-negation-elimination.md), as in part (ii).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
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
