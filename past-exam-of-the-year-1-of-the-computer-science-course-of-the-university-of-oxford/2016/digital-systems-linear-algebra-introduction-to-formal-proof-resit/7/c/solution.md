<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The derived [proof by contradiction](../../../../../reductio-ad-absurdum.md) rule is

$$
\frac{\Gamma,\neg\phi\vdash\bot}{\Gamma\vdash\phi}\quad\mathrm{RAA},
$$

where the displayed assumption $\neg\phi$ is discharged. Replace each use by [negation introduction](../../../../../negation-introduction-rule.md), giving $\Gamma\vdash\neg\neg\phi$, followed by [double-negation elimination](../../../../../double-negation-elimination.md), giving $\Gamma\vdash\phi$. Applying this replacement recursively removes all RAA occurrences while preserving the final conclusion and open premises. This uses the classical double-negation rule already supplied in the paper; it is not a general derivation of classical RAA from intuitionistic rules alone.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
