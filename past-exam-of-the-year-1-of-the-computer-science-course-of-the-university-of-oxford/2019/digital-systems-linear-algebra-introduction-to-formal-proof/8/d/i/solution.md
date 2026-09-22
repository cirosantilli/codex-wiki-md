<h1 id="8/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expand three cases as two applications of [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md). For the association $(\phi\lor\psi)\lor\rho$, the first outer branch assumes $\phi\lor\psi$ and applies the given $\phi$ and $\psi$ subproofs to obtain $\kappa$. The other outer branch is the given $\rho$ subproof. In schematic [natural deduction](../../../../../../natural-deduction.md) form:

```
1  (φ ∨ ψ) ∨ ρ                         given
2  | φ ∨ ψ                             first outer case
3  | | φ                               first inner case
4  | | κ                               given φ-subproof
5  | | ψ                               second inner case
6  | | κ                               given ψ-subproof
7  | κ                                 ∨-elim, 2, cases 3–4 and 5–6
8  | ρ                                 second outer case
9  | κ                                 given ρ-subproof
10 κ                                   ∨-elim, 1, cases 2–7 and 8–9
```

All three case assumptions are discharged and common surrounding assumptions remain. If the original three-way [logical disjunction](../../../../../../logical-disjunction.md) is parsed as $\phi\lor(\psi\lor\rho)$, use the $\phi$ subproof as the first outer branch and eliminate $\psi\lor\rho$ inside the second. Thus either binary association has the asserted [three-case disjunction elimination](../../../../../../three-case-disjunction-elimination.md), without presupposing an unproved [associativity](../../../../../../associative-property.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
