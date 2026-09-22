<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose all auxiliary bound variables fresh for the [free variables](../../../../../free-variable.md) of $p,q,r$; [alpha equivalence](../../../../../alpha-equivalence.md) permits this. The operation $\bullet$ is [composition of lambda terms](../../../../../composition-of-lambda-terms.md), so expand its definition and use [beta reduction](../../../../../beta-reduction.md):

$$
\begin{aligned}
(p\bullet q)\bullet r
&\equiv\lambda x.(\lambda y.p(qy))(rx)
\longrightarrow_\beta\lambda x.p(q(rx)),\\
p\bullet(q\bullet r)
&\equiv\lambda x.p((\lambda y.q(ry))x)
\longrightarrow_\beta\lambda x.p(q(rx)).
\end{aligned}
$$

The two [lambda terms](../../../../../lambda-term.md) have the same reduct, up to [alpha equivalence](../../../../../alpha-equivalence.md), hence they are related by [beta equivalence](../../../../../beta-equivalence.md):

$$
\boxed{(p\bullet q)\bullet r=_\beta p\bullet(q\bullet r).}
$$

No [eta conversion](../../../../../eta-conversion.md) is needed for this associativity calculation.

## ↑ Ancestors (11)

1. [A](../a.md)
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
