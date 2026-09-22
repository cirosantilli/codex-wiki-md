<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $D(\phi,\psi)=\neg(\neg\phi\land\neg\psi)$. We derive the two [disjunction introduction rules](../../../../../../disjunction-introduction-rule.md) and the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) without using any disjunction rule inside the derivations.

For left introduction, start with $\phi$ and temporarily assume $\neg\phi\land\neg\psi$. The [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) gives $\neg\phi$, and the [negation elimination rule](../../../../../../negation-elimination-rule.md) gives $\bot$. Discharge the temporary conjunction by the [negation introduction rule](../../../../../../negation-introduction-rule.md), concluding $D(\phi,\psi)$. For right introduction, start with $\psi$ and use the right [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) to obtain $\neg\psi$ instead. Thus either input derives the required encoded disjunction.

For elimination, suppose $D(\phi,\psi)$ is available, together with a derivation of $\kappa$ from an additional assumption $\phi$ and a derivation of $\kappa$ from an additional assumption $\psi$. Keep their common external context fixed. Temporarily assume $\neg\kappa$ under label $a$. Temporarily assume $\phi$ under label $b$ and insert the supplied first branch derivation to obtain $\kappa$. [Negation elimination rule](../../../../../../negation-elimination-rule.md) gives $\bot$, so [negation introduction rule](../../../../../../negation-introduction-rule.md) discharges $b$ and gives $\neg\phi$. Repeat with a temporary assumption $\psi$ under label $c$ and the supplied second branch derivation, discharging $c$ to obtain $\neg\psi$.

[Conjunction introduction rule](../../../../../../conjunction-introduction-rule.md) now gives $\neg\phi\land\neg\psi$. Its negation $D(\phi,\psi)$ gives $\bot$ by [negation elimination rule](../../../../../../negation-elimination-rule.md). The supplied [reductio ad absurdum](../../../../../../reductio-ad-absurdum.md) rule discharges $a$ and yields **$\kappa$**. This discharges the two branch assumptions as required and proves the encoded elimination rule. Its last step uses [classical propositional logic](../../../../../../classical-propositional-logic.md); the same encoded elimination principle is not generally available in [Intuitionistic propositional logic](../../../../../../intuitionistic-propositional-logic.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
