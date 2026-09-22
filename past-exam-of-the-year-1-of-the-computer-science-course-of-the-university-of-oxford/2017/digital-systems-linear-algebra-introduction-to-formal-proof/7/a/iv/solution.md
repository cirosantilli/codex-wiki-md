<h1 id="7/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use a [biconditional introduction rule](../../../../../../biconditional-introduction-rule.md) that discharges the two displayed temporary assumptions:

$$
\boxed{\frac{\Gamma,A\vdash B\qquad\Gamma,B\vdash A}{\Gamma\vdash A\leftrightarrow B}.}
$$

Suitable elimination rules are

$$
\boxed{\frac{\Gamma\vdash A\leftrightarrow B\qquad\Gamma\vdash A}{\Gamma\vdash B},\qquad
\frac{\Gamma\vdash A\leftrightarrow B\qquad\Gamma\vdash B}{\Gamma\vdash A}.}
$$

These are equivalent to using the [biconditional elimination rule](../../../../../../biconditional-elimination-rule.md) to extract the two implications and then applying [modus ponens rule](../../../../../../implication-elimination-rule.md). Together they express both directions, with no extra arbitrary assumption retained after introduction.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
