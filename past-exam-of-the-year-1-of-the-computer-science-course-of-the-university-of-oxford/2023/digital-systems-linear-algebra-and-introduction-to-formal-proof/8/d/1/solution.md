<h1 id="8/d/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use broad scope up to the enclosing parenthesis, consistent with (c). Thus the first conjunct is read as

$$
\forall x\left(P(x,y,z)\lor
\exists t\bigl(Q(z,t)\land Q(f(x,y),f(z,z))\bigr)\right).
$$

**$f(u,t)$ is not [free for substitution](../../../../../../free-for-substitution.md) for $z$.** The free occurrence of $z$ in $Q(z,t)$ lies under $\exists t$; inserting $f(u,t)$ there would capture its $t$. Rename that [bound variable](../../../../../../bound-variable.md) to a fresh $s$ first, using [alpha equivalence](../../../../../../alpha-equivalence.md). The [capture-avoiding first-order substitution](../../../../../../capture-avoiding-first-order-substitution.md) is then

$$
\boxed{\forall x\left(P(x,y,f(u,t))\lor
\exists s\left(Q(f(u,t),s)\land
Q\bigl(f(x,y),f(f(u,t),f(u,t))\bigr)\right)\right)
\land\exists y\,Q(y,y).}
$$

Every occurrence of $z$ in the original formula is free, so all four are replaced. The variable $t$ introduced by the term remains free, and the final $\exists y\,Q(y,y)$ is unchanged.

## ↑ Ancestors (14)

1. [1](../1.md)
2. [D](../../d.md)
3. [8](../../../8.md)
4. [Introduction to formal proof](../../../introduction-to-formal-proof.md)
5. [Digital systems, linear algebra and introduction to formal proof](../../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
6. [2023](../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
