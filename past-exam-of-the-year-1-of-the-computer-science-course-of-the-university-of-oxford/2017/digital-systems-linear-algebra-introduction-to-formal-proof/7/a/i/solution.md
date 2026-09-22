<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [conjunction elimination](../../../../../../conjunction-elimination-rule.md) to obtain both premises needed for a contradiction under a temporary implication assumption. The following [natural deduction](../../../../../../natural-deduction.md) derivation discharges precisely assumption 4:

$$
\begin{array}{rll}
1&Q\land P&\text{premise}\\
2&P&\land E\ 1\\
3&Q&\land E\ 1\\
4&\quad P\to\neg Q&\text{assumption}\\
5&\quad\neg Q&\to E\ 4,2\\
6&\quad\bot&\neg E\ 3,5\\
7&\neg(P\to\neg Q)&\neg I\ 4\text{--}6
\end{array}
$$

Here $\to E$ is the [implication elimination rule](../../../../../../implication-elimination-rule.md) and $\neg I$ is [negation introduction](../../../../../../negation-introduction-rule.md). The original conjunction remains the only undischarged premise.

## ↑ Ancestors (13)

1. [I](../i.md)
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
