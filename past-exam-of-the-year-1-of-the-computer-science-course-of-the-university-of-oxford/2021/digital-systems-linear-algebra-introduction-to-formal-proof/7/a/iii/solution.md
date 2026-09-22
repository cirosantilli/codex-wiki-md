<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) on the outer disjunction. In its left branch, assume $P\lor Q$ and apply the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) again: from a case assumption $P$, the [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) gives $P\lor R$; from a case assumption $Q$, the premise $Q\to R$ and the [modus ponens rule](../../../../../../implication-elimination-rule.md) give $R$, then the [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) gives $P\lor R$. Discharging those two inner case assumptions yields $P\lor R$ under the left outer branch.

In the right outer branch, assume $R\lor S$. A case assumption $R$ gives $P\lor R$ by the [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md). A case assumption $S$, together with the premise $\neg S$, gives $\bot$ by the [negation elimination rule](../../../../../../negation-elimination-rule.md), and then $P\lor R$ by [logical falsity elimination rule](../../../../../../logical-falsity-elimination-rule.md). Discharge these inner case assumptions with the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md).

Both outer branches now have the same conclusion. Discharge the two outer case assumptions with the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) to obtain **$P\lor R$** under exactly the stated premises.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
