<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the new [exclusive or](../../../../../../exclusive-or.md) connective as $\oplus$. Give it the two introduction rules

$$
\frac{P\quad\neg Q}{P\oplus Q}\ \oplus I_1,\qquad
\frac{\neg P\quad Q}{P\oplus Q}\ \oplus I_2,
$$

and the elimination rule

$$
\frac{P\oplus Q\qquad\Gamma,P,\neg Q\vdash K\qquad\Gamma,\neg P,Q\vdash K}{\Gamma\vdash K}\ \oplus E.
$$

In elimination, discharge the two pairs of case assumptions; retain the assumptions needed for the major premise and the shared context $\Gamma$. These are [natural deduction](../../../../../../natural-deduction.md) rules for exactly one of $P,Q$, not merely at least one.

For a syntactic check, derive $(P\land\neg Q)\lor(\neg P\land Q)$ from $P\oplus Q$ by $\oplus E$: in the first case introduce $P\land\neg Q$ and then the left disjunct; in the second case introduce $\neg P\land Q$ and then the right disjunct. Conversely, from that disjunction use [disjunction elimination](../../../../../../disjunction-elimination-rule.md); [conjunction elimination](../../../../../../conjunction-elimination-rule.md) extracts $P,\neg Q$ in the first branch and $\neg P,Q$ in the second, so the respective introduction rule yields $P\oplus Q$ in both. This proves equivalence to the ordinary truth-functional specification and explains both the introduction and elimination rules.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
