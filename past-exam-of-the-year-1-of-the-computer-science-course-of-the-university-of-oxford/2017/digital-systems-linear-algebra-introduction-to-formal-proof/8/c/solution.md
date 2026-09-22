<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The displayed proof is invalid:** its existential-elimination step exports $Q(x_0)$ while $x_0$ is still free in that conclusion. This is [witness escape](../../../../../witness-escape.md). Existential introduction afterwards cannot repair the invalid intermediate step.

Instead introduce the existential while the witness assumption is still open:

$$
\begin{array}{rll}
1&\forall x\,(P(x)\to Q(x))&\text{premise}\\
2&\exists x\,P(x)&\text{premise}\\
3&\quad P(a)&\text{fresh witness assumption}\\
4&\quad P(a)\to Q(a)&\forall E\ 1\\
5&\quad Q(a)&\to E\ 4,3\\
6&\quad\exists x\,Q(x)&\exists I\ 5\\
7&\exists x\,Q(x)&\exists E\ 2,3\text{--}6
\end{array}
$$

The [existential quantifier introduction rule](../../../../../existential-quantifier-introduction-rule.md) at line 6 removes the free witness from the exported statement, so the final [existential elimination](../../../../../existential-quantifier-elimination-rule.md) satisfies its [eigenvariable condition](../../../../../eigenvariable-condition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
