<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Let $X=C([0,T];L^2(\mathbb R))$ and define the map suggested by the [variation-of-constants formula](../../../../../../variation-of-constants-formula.md):

$$
(\Phi u)(t)=U(t,0)u_0+\int_0^tU(t,s)f(s,u(s))\,ds.
$$

The [strong continuity](../../../../../../strong-continuity.md) of the [evolution family](../../../../../../evolution-family.md) and the continuity of $f$ imply that $\Phi$ maps $X$ into itself. Because $U(t,s)$ is unitary and $\|f(t,u)\|_2\leq C$,

$$
\|\Phi u(t)\|_2\leq\|u_0\|_2+Ct.
$$

Equip $X$ with the [exponentially weighted supremum norm](../../../../../../exponentially-weighted-supremum-norm.md)

$$
\|u\|_\alpha=\sup_{0\leq t\leq T}e^{-\alpha t}\|u(t)\|_2.
$$

This equivalent norm makes $X$ a [Banach space](../../../../../../banach-space-split.md). Using that $f$ is a [globally Lipschitz function](../../../../../../globally-lipschitz-function.md) and that the [unitary operator](../../../../../../unitary-operator.md) $U(t,s)$ preserves the norm,

$$
\begin{aligned}
e^{-\alpha t}\|\Phi u(t)-\Phi v(t)\|_2
&\leq L\int_0^te^{-\alpha(t-s)}e^{-\alpha s}\|u(s)-v(s)\|_2\,ds\\
&\leq\frac{L}{\alpha}\|u-v\|_\alpha.
\end{aligned}
$$

Choose $\alpha>L$. Then $\Phi$ is a [contraction mapping](../../../../../../contraction-mapping.md), so the [Banach fixed-point theorem](../../../../../../contraction-mapping-theorem.md) gives a unique fixed point $u\in X$. This fixed point is exactly the required [mild solution of an abstract Cauchy problem](../../../../../../mild-solution-of-an-abstract-cauchy-problem.md):

$$
\boxed{u(t)=U(t,0)u_0+\int_0^tU(t,s)f(s,u(s))\,ds}.
$$

The weighted-norm argument works on the whole prescribed finite interval, so no subdivision of $[0,T]$ is needed.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
