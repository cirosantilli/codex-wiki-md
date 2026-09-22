<h1 id="16f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Von Neumann hierarchy](../../../../../../von-neumann-hierarchy.md) is defined by [transfinite recursion](../../../../../../transfinite-recursion.md):

$$
V_0=\varnothing,
\qquad
V_{\alpha+1}=\mathcal P(V_\alpha),
\qquad
V_\lambda=\bigcup_{\beta<\lambda}V_\beta
$$

for a limit ordinal $\lambda$.

We prove by [transfinite induction](../../../../../../transfinite-induction.md) that every $V_\alpha$ is a [transitive set](../../../../../../transitive-set.md). The claim is immediate for $V_0$. If $V_\alpha$ is transitive and $x\in y\in V_{\alpha+1}$, then $y\subseteq V_\alpha$, so $x\in V_\alpha$. Transitivity also gives $x\subseteq V_\alpha$, hence $x\in\mathcal P(V_\alpha)=V_{\alpha+1}$. At a limit stage, if $x\in y\in V_\lambda$, then $y\in V_\beta$ for some $\beta<\lambda$, so $x\in V_\beta\subseteq V_\lambda$.

Transitivity implies $V_\alpha\subseteq\mathcal P(V_\alpha)=V_{\alpha+1}$. Induction and unions at limit stages then give

$$
\boxed{\alpha\leq\beta\Longrightarrow V_\alpha\subseteq V_\beta}.
$$

By well-founded recursion on membership, define the [rank of a set](../../../../../../rank-of-a-set.md)

$$
\operatorname{rank}(x)
=\sup_{y\in x}\bigl(\operatorname{rank}(y)+1\bigr).
$$

Induction on this rank gives $y\in V_{\operatorname{rank}(x)}$ for every $y\in x$. Thus

$$
x\subseteq V_{\operatorname{rank}(x)}
$$

and consequently

$$
\boxed{x\in V_{\operatorname{rank}(x)+1}}.
$$

Every set therefore occurs at some level of the hierarchy.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16F](../../16f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
