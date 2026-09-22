<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

The [Von Neumann hierarchy](../../../../../von-neumann-hierarchy.md) is defined by [transfinite recursion](../../../../../transfinite-recursion.md):

$$
V_0=\varnothing,
\qquad V_{\alpha+1}=\mathcal P(V_\alpha),
\qquad V_\lambda=\bigcup_{\beta<\lambda}V_\beta
$$

for every [limit ordinal](../../../../../limit-ordinal.md) $\lambda$.

We prove simultaneously by [transfinite induction](../../../../../transfinite-induction.md) that every $V_\alpha$ is a [transitive set](../../../../../transitive-set.md) and that $V_\alpha\subseteq V_{\alpha+1}$. The claims are immediate for $V_0$. Suppose first that $V_\alpha$ is transitive. If $x\in y\in V_{\alpha+1}=\mathcal P(V_\alpha)$, then $y\subseteq V_\alpha$, so $x\in V_\alpha$. Moreover, transitivity says that every $x\in V_\alpha$ satisfies $x\subseteq V_\alpha$, and hence

$$
x\in\mathcal P(V_\alpha)=V_{\alpha+1}.
$$

Thus $V_{\alpha+1}$ is transitive and $V_\alpha\subseteq V_{\alpha+1}$. At a limit $\lambda$, if $x\in y\in V_\lambda$, then $y\in V_\beta$ for some $\beta<\lambda$; transitivity of $V_\beta$ gives $x\in V_\beta\subseteq V_\lambda$. The inclusions at successor stages also imply

$$
\boxed{V_\alpha\subseteq V_\beta\quad\text{whenever }\alpha\leq\beta.}
$$

Finally, the [rank of a set](../../../../../rank-of-a-set.md) $x$ is the [ordinal](../../../../../ordinal.md)

$$
\operatorname{rank}(x)=\sup_{y\in x}\bigl(\operatorname{rank}(y)+1\bigr).
$$

Every $y\in x$ belongs to $V_{\operatorname{rank}(y)+1}\subseteq V_{\operatorname{rank}(x)}$, so $x\subseteq V_{\operatorname{rank}(x)}$. Therefore

$$
\boxed{x\in V_{\operatorname{rank}(x)+1},}
$$

which proves that every set occurs in the hierarchy.

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
