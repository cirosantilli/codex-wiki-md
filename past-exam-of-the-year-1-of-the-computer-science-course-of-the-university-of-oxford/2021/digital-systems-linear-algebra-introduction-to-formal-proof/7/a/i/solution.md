<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [natural deduction](../../../../../../natural-deduction.md) with labelled temporary assumptions. Assume $\neg P\to\neg Q$ under label $a$, then $\neg P\to Q$ under label $b$, then $\neg P$ under label $c$. Two applications of the [modus ponens rule](../../../../../../implication-elimination-rule.md) give $\neg Q$ and $Q$. The [negation elimination rule](../../../../../../negation-elimination-rule.md) gives $\bot$, and the supplied [reductio ad absurdum](../../../../../../reductio-ad-absurdum.md) rule discharges $c$ to conclude $P$.

Discharge $b$ using the [implication introduction rule](../../../../../../implication-introduction-rule.md), obtaining $(\neg P\to Q)\to P$ under $a$. Discharge $a$ with the [implication introduction rule](../../../../../../implication-introduction-rule.md), obtaining

$$
(\neg P\to\neg Q)\to((\neg P\to Q)\to P).
$$

All three temporary assumptions have now been discharged; no premise remains.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
