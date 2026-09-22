<h1 id="a/1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Fix the particular occurrence of $\alpha$ that is being replaced. The [subformula](../../../../../subformula.md) analysis above makes it a node of the [formula syntax tree](../../../../../syntax-tree-of-a-formula.md) of $\phi$. Proceed by [structural induction](../../../../../structural-induction.md) on the surrounding [logical formula](../../../../../logical-formula.md).

If this node is the root, the [subformula replacement](../../../../../subformula-replacement.md) gives $\beta$, already a [logical formula](../../../../../logical-formula.md). Otherwise, if $\phi=\neg\psi$, the chosen occurrence lies inside $\psi$. The induction hypothesis gives a [logical formula](../../../../../logical-formula.md) $\psi'$ after the [subformula replacement](../../../../../subformula-replacement.md) there, and the whole result is the [logical formula](../../../../../logical-formula.md) $\neg\psi'$. If $\phi=(\psi\to\chi)$, a proper chosen occurrence lies in exactly one of the two children. Replacing inside that child gives either $(\psi'\to\chi)$ or $(\psi\to\chi')$, each a [logical formula](../../../../../logical-formula.md) by the [formation rule](../../../../../formation-rule.md). A [logical variable](../../../../../logical-variable.md) has no proper [subformula](../../../../../subformula.md), so there is no additional base case.

Therefore **replacing the designated [subformula occurrence](../../../../../subformula-occurrence.md) by any [logical formula](../../../../../logical-formula.md) preserves well-formedness**. The argument concerns one chosen occurrence; it does not require simultaneous [subformula replacement](../../../../../subformula-replacement.md) of every occurrence of the same string.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
