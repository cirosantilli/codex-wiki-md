<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For [implication creation rule](../../../../../implication-creation-rule.md), keep $\psi$ available and discharge an otherwise unused antecedent:

```
1  ψ                         given
2  | φ                       assume
3  | ψ                       available from 1
4  φ → ψ                     →-intro, discharge 2–3
```

For [implication distribution rule](../../../../../implication-distribution-rule.md), write $H=\phi\to(\psi\to\rho)$. The [logical derivation](../../../../../logical-derivation.md) below keeps $H$ available and discharges exactly the two [temporary assumptions](../../../../../temporary-assumption.md):

```
1  φ → (ψ → ρ)                          given
2  | φ → ψ                              assume
3  | | φ                                assume
4  | | ψ                                →-elim, 3 and 2
5  | | ψ → ρ                            →-elim, 3 and 1
6  | | ρ                                →-elim, 4 and 5
7  | φ → ρ                              →-intro, discharge 3–6
8  (φ → ψ) → (φ → ρ)                    →-intro, discharge 2–7
```

These justify both [derived inference rules](../../../../../derived-inference-rule.md) using Figure 2 primitives. Their rule forms retain any other surrounding assumptions; they are not unconditionally asserted conclusions after the displayed numerator is forgotten.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
