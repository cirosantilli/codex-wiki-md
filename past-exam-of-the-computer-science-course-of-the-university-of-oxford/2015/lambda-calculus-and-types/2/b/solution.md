<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $\star$ as the domain of the new [function type](../../../../../function-type.md). Since $x\notin\operatorname{Subjects}(\Gamma)$, the assumption $x:\star$ is consistent with $\Gamma$ and deleting $x$ leaves $\Gamma$ unchanged. The [lambda abstraction](../../../../../lambda-abstraction.md) rule gives

$$
\frac{\Gamma\mapsto p:A}
{\Gamma\mapsto\lambda x.p:\star\Rightarrow A}.
$$

Use the [universal typing axiom](../../../../../universal-typing-axiom.md) for $q$, then the [lambda application](../../../../../lambda-application.md) rule:

$$
\frac{\Gamma\mapsto\lambda x.p:\star\Rightarrow A
\qquad\varnothing\mapsto q:\star}
{\Gamma\mapsto(\lambda x.p)q:A}.
$$

Therefore

$$
\boxed{\Gamma\mapsto(\lambda x.p)q:A\quad\text{for every }q.}
$$

The condition is about the [typing context](../../../../../typing-context.md), not the [free variables](../../../../../free-variable.md) of $p$. Some occurrences of $x$ in $p$ might have been hidden by a use of the [universal typing axiom](../../../../../universal-typing-axiom.md); the derivation above still follows the printed rules.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
