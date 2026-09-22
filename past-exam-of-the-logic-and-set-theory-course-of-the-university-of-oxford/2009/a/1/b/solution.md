<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A term $t$ is [free for substitution](../../../../../free-for-substitution.md) for $x_i$ in $\alpha$ when none of its variables becomes bound at a free occurrence of $x_i$ being replaced. Equivalently, no [quantifier](../../../../../quantifier.md) surrounding such an occurrence binds a variable of $t$. Bound occurrences of $x_i$ are not replaced. This occurrence-sensitive condition prevents variable capture.

For example take $\alpha(x)=\exists y\,\neg(x=y)$ and $t=y$. On a two-element domain, $\forall x\exists y\,\neg(x=y)$ is true. Naive textual substitution produces $\exists y\,\neg(y=y)$, which is false on every nonempty domain. Thus the corresponding unrestricted A4 implication would be invalid. The problem is that the inserted free $y$ was captured by the existing [existential quantifier](../../../../../existential-quantification.md). Renaming that binder first instead gives the correct instance $\exists z\,\neg(y=z)$, with $z$ fresh.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
