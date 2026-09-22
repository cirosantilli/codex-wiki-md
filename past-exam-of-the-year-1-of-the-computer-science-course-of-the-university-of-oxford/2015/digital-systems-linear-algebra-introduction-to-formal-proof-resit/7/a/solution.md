<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [implication introduction rule](../../../../../implication-introduction-rule.md) opens a [subproof](../../../../../subproof.md) under a [temporary assumption](../../../../../temporary-assumption.md) $\phi$, derives $\psi$, then performs [assumption discharge](../../../../../assumption-discharge.md) to conclude $\phi\to\psi$. The [negation introduction rule](../../../../../negation-introduction-rule.md) instead derives [logical falsity](../../../../../logical-falsity.md) $\bot$ under a [temporary assumption](../../../../../temporary-assumption.md) $\phi$, discharges it, and concludes $\neg\phi$:

$$
\boxed{\frac{\Gamma,\phi\vdash\psi}{\Gamma\vdash\phi\to\psi}
\qquad
\frac{\Gamma,\phi\vdash\bot}{\Gamma\vdash\neg\phi}.}
$$

The rectangular boxes delimit these [subproofs](../../../../../subproof.md) and the scope of their [temporary assumptions](../../../../../temporary-assumption.md). A line depending on the boxed [temporary assumption](../../../../../temporary-assumption.md) cannot simply be used outside the box. The relevant introduction rule exports the indicated [logical implication](../../../../../logical-implication.md) or [negation](../../../../../negation.md); other surrounding assumptions $\Gamma$ stay in force.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
