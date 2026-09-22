<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The occurrence of $y$ in $P(x,y)$ lies under the quantifier $\exists x$. Directly inserting the term $x+z$ would capture its free $x$: the result $\exists x\,P(x,x+z)$ would make the inserted $x$ bound and change the intended dependence on the original free value. Therefore the term is not free for the literal substitution requested.

Perform [capture-avoiding first-order substitution](../../../../../capture-avoiding-first-order-substitution.md) by first renaming [bound variables](../../../../../bound-variable.md) to fresh names. Renaming the first binder to $u$ is necessary; renaming the second to $v$ is optional but makes the result especially clear. These renamings give the equivalent formula $(\exists u\,P(u,y))\lor(\exists v\,Q(v))$. Substituting only the free occurrences of $y$ now gives

$$
\boxed{(\exists u\,P(u,x+z))\lor(\exists v\,Q(v)).}
$$

Both $x$ and $z$ in the inserted term remain [free variables](../../../../../free-variable.md). The original $\exists z$ has scope only over its own disjunct and would not capture the inserted $z$ in the first disjunct; its optional renaming is not a necessary capture repair. This distinction avoids confusing reuse of a letter elsewhere with binding within the relevant scope.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
