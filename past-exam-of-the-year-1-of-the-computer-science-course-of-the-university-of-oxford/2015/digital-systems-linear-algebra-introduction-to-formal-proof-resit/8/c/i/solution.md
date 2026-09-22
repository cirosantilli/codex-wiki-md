<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [equality introduction rule](../../../../../../equality-introduction-rule.md) is reflexivity, with no premise. The [equality elimination rule](../../../../../../equality-elimination-rule.md) is substitution of equal [first-order terms](../../../../../../first-order-term.md) into a [first-order formula](../../../../../../first-order-formula.md):

$$
\boxed{\frac{}{\Gamma\vdash t=t}\ =I,\qquad
\frac{\Gamma\vdash s=t\qquad\Gamma\vdash\phi(s)}{\Gamma\vdash\phi(t)}\ =E.}
$$

The indicated substitution must be [capture-avoiding substitution in first-order logic](../../../../../../capture-avoiding-first-order-substitution.md): the [first-order terms](../../../../../../first-order-term.md) must be free for the replaced variable. One can designate a particular argument occurrence by choosing $\phi(v)$ appropriately; the rule does not demand replacing every occurrence of an identical-looking term in a formula.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
