<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $I\equiv\lambda u.u$ for the [I combinator](../../../../../i-combinator.md), and choose $x$ outside the [free variables](../../../../../free-variable.md) of $p$. Both orders of [composition of lambda terms](../../../../../composition-of-lambda-terms.md) first give the same [lambda abstraction](../../../../../lambda-abstraction.md) by [beta reduction](../../../../../beta-reduction.md):

$$
\begin{aligned}
p\bullet I&\equiv\lambda x.p((\lambda u.u)x)
\longrightarrow_\beta\lambda x.px,\\
I\bullet p&\equiv\lambda x.(\lambda u.u)(px)
\longrightarrow_\beta\lambda x.px.
\end{aligned}
$$

The freshness condition is exactly the side condition for [eta conversion](../../../../../eta-conversion.md), which contracts $\lambda x.px$ to $p$. Therefore

$$
\boxed{p\bullet I=_{\beta\eta}p=_{\beta\eta}I\bullet p.}
$$

Here [eta conversion](../../../../../eta-conversion.md) matters: a [free variable](../../../../../free-variable.md) $p$ is already in [beta-normal form](../../../../../beta-normal-form.md), as is $\lambda x.px$, and [beta equivalence](../../../../../beta-equivalence.md) alone does not equate them.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
