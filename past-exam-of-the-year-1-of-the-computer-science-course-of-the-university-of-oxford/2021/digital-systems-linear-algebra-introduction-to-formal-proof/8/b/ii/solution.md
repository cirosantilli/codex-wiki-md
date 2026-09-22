<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $u$ be fresh, not free in any of the three universal premises. [Universal quantifier elimination rule](../../../../../../universal-quantifier-elimination-rule.md) gives $\neg P(u)\lor R(c,u)$, $Q(u)\to R(c,u)$ and $P(u)\lor Q(u)$. Apply [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) to the last formula.

In the $P(u)$ branch, apply [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) to $\neg P(u)\lor R(c,u)$. Its $\neg P(u)$ case contradicts $P(u)$ by [negation elimination rule](../../../../../../negation-elimination-rule.md), and [logical falsity elimination rule](../../../../../../logical-falsity-elimination-rule.md) then gives $R(c,u)$. Its $R(c,u)$ case already gives that conclusion. Discharge those two inner case assumptions to obtain $R(c,u)$ under the outer $P(u)$ assumption. In the outer $Q(u)$ branch, the [modus ponens rule](../../../../../../implication-elimination-rule.md) applied to $Q(u)\to R(c,u)$ gives $R(c,u)$ directly.

Discharge the two outer case assumptions by [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md). The conclusion $R(c,u)$ now depends only on the universal premises, in which $u$ is not free. [Universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) therefore gives **$\forall x\,R(c,x)$**. All case assumptions have been discharged, and the argument requires no classical [reductio ad absurdum](../../../../../../reductio-ad-absurdum.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
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
