<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [variable](../../../../../../variable-mathematics.md) $v$ is fresh for the surrounding context $\Gamma$ when it does not occur free in any undischarged assumption in $\Gamma$. Choose it also distinct from bound variables that would cause [variable capture](../../../../../../variable-capture.md) in the intended substitution. The [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) is

$$
\boxed{\frac{\Gamma\vdash\phi(v)}{\Gamma\vdash\forall x\,\phi(x)}\quad(v\text{ fresh for }\Gamma).}
$$

Its justification is that the [logical derivation](../../../../../../logical-derivation.md) of $\phi(v)$ used no special information about $v$, so it establishes the property of an arbitrary object. Semantically, changing the assignment of $v$ preserves the truth of $\Gamma$; therefore $\phi(v)$ holds for every possible assigned object. Without the [eigenvariable condition](../../../../../../eigenvariable-condition.md), the assumption $R(v)$ could incorrectly be generalized to $\forall x\,R(x)$ in an interpretation where only one of two objects satisfies $R$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
