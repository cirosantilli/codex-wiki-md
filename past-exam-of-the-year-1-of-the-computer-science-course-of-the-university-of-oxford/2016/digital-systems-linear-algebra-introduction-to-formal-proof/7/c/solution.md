<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Proof by contradiction](../../../../../reductio-ad-absurdum.md), or [reductio ad absurdum](../../../../../reductio-ad-absurdum.md), has the form

$$
\boxed{\frac{\Gamma,\neg\phi\vdash\bot}{\Gamma\vdash\phi}\quad\mathrm{RAA},}
$$

discharging the assumption $\neg\phi$. This is the classical rule that concludes $\phi$ directly, as opposed to the [negation introduction rule](../../../../../negation-introduction-rule.md), which concludes a negation.

To derive [double-negation elimination](../../../../../double-negation-elimination.md) using RAA without assuming [double-negation elimination](../../../../../double-negation-elimination.md) itself, use
```
1  ¬¬φ   premise
2  | ¬φ  assumption
3  | ⊥   ¬-elim 2,1
4  φ     RAA 2–3
```
Here line 1 is the negation of line 2. Thus only [negation elimination rule](../../../../../negation-elimination-rule.md) inside the [subproof](../../../../../subproof.md), followed by RAA, is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
