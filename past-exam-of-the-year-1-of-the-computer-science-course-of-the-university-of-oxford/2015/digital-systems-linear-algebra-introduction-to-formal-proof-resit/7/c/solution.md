<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The classical [proof by contradiction](../../../../../reductio-ad-absurdum.md) rule, also called reductio ad absurdum, is

$$
\boxed{\frac{\Gamma,\neg\phi\vdash\bot}{\Gamma\vdash\phi}\ \mathrm{RAA},}
$$

with [assumption discharge](../../../../../assumption-discharge.md) of the displayed $\neg\phi$. It differs from the [negation introduction rule](../../../../../negation-introduction-rule.md) by concluding $\phi$ from a contradictory assumption of its [negation](../../../../../negation.md).

To derive [double-negation elimination](../../../../../double-negation-elimination.md) using this rule, start with $\neg\neg\phi$, assume $\neg\phi$, and apply the [negation elimination rule](../../../../../negation-elimination-rule.md) to those two formulas:

$$
\begin{array}{rll}
1&\neg\neg\phi&\text{premise}\\
2&[\neg\phi]^a&\text{assumption}\\
3&\quad\bot&\neg E\ 2,1\\
4&\phi&\mathrm{RAA}\ (2\text{--}3).
\end{array}
$$

No [double-negation elimination](../../../../../double-negation-elimination.md) occurs inside this derivation, so the argument is not circular.

## ↑ Ancestors (12)

1. [C](../c.md)
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
