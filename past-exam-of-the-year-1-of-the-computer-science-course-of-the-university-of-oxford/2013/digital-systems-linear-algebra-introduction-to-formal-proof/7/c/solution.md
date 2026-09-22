<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [proof by contradiction](../../../../../reductio-ad-absurdum.md), assume the [negation](../../../../../negation.md) of a desired conclusion $A$, derive [logical falsity](../../../../../logical-falsity.md), and discharge the assumption to infer $A$. A rule expressing this is

$$
\boxed{\frac{\begin{array}{c}[\neg A]^i\\\vdots\\\bot\end{array}}{A}\;\mathrm{RAA}\;(i).}
$$

Here the label $i$ identifies the assumption being discharged; any other open assumptions remain.

To derive this rule using the supplied rules, apply [negation introduction](../../../../../negation-introduction-rule.md) to the [subproof](../../../../../subproof.md) from $\neg A$ to $\bot$. This discharges $\neg A$ and yields $\neg\neg A$. Apply [double-negation elimination](../../../../../double-negation-elimination.md) to obtain $A$. Thus the extra rule is admissible because Figure 1 explicitly includes [double-negation elimination](../../../../../double-negation-elimination.md).[Printed p. 9, Figure 1, double-negation elimination](../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2013.md)

This is the classical form of [proof by contradiction](../../../../../reductio-ad-absurdum.md); simply deriving $\neg A$ from an assumption $A$ leading to [logical falsity](../../../../../logical-falsity.md) uses [negation introduction](../../../../../negation-introduction-rule.md) alone.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
