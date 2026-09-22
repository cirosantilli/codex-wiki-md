<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $N(\phi,\psi)$ abbreviate $\neg\phi\land\neg\psi$. Suitable rules are

$$
\frac{\neg\phi\qquad\neg\psi}{N(\phi,\psi)}\;N\mathrm I,\qquad
\frac{N(\phi,\psi)}{\neg\phi}\;N\mathrm E_L,\qquad
\frac{N(\phi,\psi)}{\neg\psi}\;N\mathrm E_R.
$$

Their derivations require no new axiom. For introduction, apply the [conjunction introduction rule](../../../../../../conjunction-introduction-rule.md) to the two premises, obtaining $\neg\phi\land\neg\psi$, which is exactly the abbreviation. For left and right elimination, unfold the abbreviation and apply the corresponding [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md). These are therefore derived rules for the NOR connective.

An equivalent subproof presentation of introduction permits one subproof from assumption $\phi$ to $\bot$ and another from assumption $\psi$ to $\bot$: use the [negation introduction rule](../../../../../../negation-introduction-rule.md) to discharge each assumption, then apply the [conjunction introduction rule](../../../../../../conjunction-introduction-rule.md). If elimination is desired in [contradiction](../../../../../../contradiction.md) form, combine the left projection with $\phi$, or the right projection with $\psi$, using the [negation elimination rule](../../../../../../negation-elimination-rule.md). All these presentations reduce directly to the permitted rules.

## ↑ Ancestors (13)

1. [I](../i.md)
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
