<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [natural deduction](../../../../../../natural-deduction.md), [conjunction introduction](../../../../../../conjunction-introduction-rule.md) combines derivations of $\phi$ and $\psi$ under the available assumptions into $\phi\land\psi$. [Disjunction elimination](../../../../../../disjunction-elimination-rule.md) takes $\phi\lor\psi$ and two [subproofs](../../../../../../subproof.md) of the same conclusion $\kappa$, one assuming $\phi$ and the other assuming $\psi$, and concludes $\kappa$. [Implication introduction](../../../../../../implication-introduction-rule.md) takes a [subproof](../../../../../../subproof.md) deriving $\psi$ from a [temporary assumption](../../../../../../temporary-assumption.md) $\phi$, and concludes $\phi\to\psi$.

The rectangular boxes mark the scopes of [temporary assumptions](../../../../../../temporary-assumption.md). The [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) discharges its two case assumptions, while the [implication introduction rule](../../../../../../implication-introduction-rule.md) discharges the antecedent assumption. Other surrounding assumptions remain in force; intermediate results depending on the boxed assumptions cannot be exported arbitrarily. Schematically,

$$
\boxed{\frac{\phi\quad\psi}{\phi\land\psi},\qquad\frac{\phi\lor\psi\quad[\phi]\ \vdots\ \kappa\quad[\psi]\ \vdots\ \kappa}{\kappa},\qquad\frac{[\phi]\ \vdots\ \psi}{\phi\to\psi}.}
$$

Here the square brackets designate the assumptions discharged by the corresponding [inference rule](../../../../../../inference-rule.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
