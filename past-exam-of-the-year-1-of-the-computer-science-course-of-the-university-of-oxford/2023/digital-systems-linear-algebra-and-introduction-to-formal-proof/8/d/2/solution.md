<h1 id="8/d/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Under the same scope convention, **$g(t,z)$ is not [free for substitution](../../../../../../free-for-substitution.md) for $y$**. The occurrence of $y$ inside $Q(f(x,y),f(z,z))$ is free but lies under $\exists t$, so its replacement would capture the new $t$. Rename this binder to fresh $s$. Substitute only for the free $y$ occurrences in the first conjunct:

$$
\boxed{\forall x\left(P(x,g(t,z),z)\lor
\exists s\left(Q(z,s)\land
Q\bigl(f(x,g(t,z)),f(z,z)\bigr)\right)\right)
\land\exists y\,Q(y,y).}
$$

The two occurrences of $y$ in the final conjunct are [bound variables](../../../../../../bound-variable.md) and remain unchanged. The inserted $t,z$ remain free.

If instead one gives the printed $\exists t$ only the scope $Q(z,t)$, this part's free-for-substitution answer becomes **yes**, because neither free $y$ occurrence then lies under that binder. Under that alternative parsing, the result is explicitly

$$
\forall x\left(P(x,g(t,z),z)\lor
\left((\exists t\,Q(z,t))\land Q(f(x,g(t,z)),f(z,z))\right)\right)
\land\exists y\,Q(y,y).
$$

The narrower reading does not change the negative answer in (1): its occurrence of $z$ inside $Q(z,t)$ still requires renaming that binder before substitution. The broad-scope answers above give a single consistent parsing across the paper.

## ↑ Ancestors (14)

1. [2](../2.md)
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
