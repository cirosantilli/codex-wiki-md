<h1 id="8/f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The term $x+z$ is not [free for substitution](../../../../../../free-for-substitution.md) for $y$.** The occurrence of $y$ in $x<y$ is under $\exists x$, which would capture the inserted $x$. The other occurrence, in the outside disjunct $y<z$, has no enclosing [quantifier](../../../../../../quantifier.md). The inner $\forall z$ does not bind the occurrence of $y$ in its antecedent, so it creates no additional capture at that substitution site.

Rename the bound $x$ to a fresh $u$, then carry out [capture-avoiding first-order substitution](../../../../../../capture-avoiding-first-order-substitution.md). The result is

$$
\boxed{\varphi[x+z/y]=\bigl(\exists u\,(u<x+z\to\forall z\,(u<z+2))\bigr)\lor(x+z<z).}
$$

The inserted $z$ in $u<x+z$ remains free because it lies outside the scope of $\forall z$. One may additionally rename that bound $z$ for readability, but it is not necessary for correctness.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [F](../../f.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
