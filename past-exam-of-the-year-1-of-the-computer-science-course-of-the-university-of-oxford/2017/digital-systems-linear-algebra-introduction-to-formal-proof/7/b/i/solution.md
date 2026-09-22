<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the two implications in turn, then derive a contradiction from $\neg P$. The [natural deduction](../../../../../../natural-deduction.md) proof is

$$
\begin{array}{rll}
1&\quad\neg P\to Q&\text{assumption}\\
2&\qquad\neg P\to\neg Q&\text{assumption}\\
3&\qquad\quad\neg P&\text{assumption}\\
4&\qquad\quad Q&\to E\ 1,3\\
5&\qquad\quad\neg Q&\to E\ 2,3\\
6&\qquad\quad\bot&\neg E\ 4,5\\
7&\qquad P&\mathrm{RAA}\ 3\text{--}6\\
8&\quad(\neg P\to\neg Q)\to P&\to I\ 2\text{--}7\\
9&(\neg P\to Q)\to((\neg P\to\neg Q)\to P)&\to I\ 1\text{--}8
\end{array}
$$

Here RAA is the derived [proof by contradiction](../../../../../../reductio-ad-absurdum.md) rule. The last two [assumption discharge](../../../../../../assumption-discharge.md) steps establish the requested right-associated implication as a theorem.

## ↑ Ancestors (13)

1. [I](../i.md)
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
