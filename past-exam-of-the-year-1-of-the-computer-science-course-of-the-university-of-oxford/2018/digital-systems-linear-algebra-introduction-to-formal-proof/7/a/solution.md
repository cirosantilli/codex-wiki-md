<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [reductio ad absurdum](../../../../../reductio-ad-absurdum.md) rule discharges an assumption $\neg\phi$ from a derivation of contradiction and concludes $\phi$. It is derivable using [negation introduction](../../../../../negation-introduction-rule.md) followed by [double-negation elimination](../../../../../double-negation-elimination.md):

$$
\frac{\Gamma,\neg\phi\vdash\bot}{\Gamma\vdash\neg\neg\phi}\ \neg I,\qquad
\frac{\Gamma\vdash\neg\neg\phi}{\Gamma\vdash\phi}\ \neg\neg E.
$$

Conversely, if RAA is supplied, [double-negation elimination](../../../../../double-negation-elimination.md) follows from this [natural deduction](../../../../../natural-deduction.md) derivation:
```
1. ¬¬φ                  premise
2.   ¬φ                 assumption [i]
3.   ⊥                  ¬E, 1, 2
4. φ                    RAA, 2–3, discharging [i]
```
Thus replacing double-negation elimination by RAA leaves these classical deductions available. RAA is not being assumed as an intuitionistic rule.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
