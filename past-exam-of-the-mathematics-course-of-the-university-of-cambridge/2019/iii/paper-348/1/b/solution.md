<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Given any admissible [transport map](../../../../../../transport-map.md) $T$, form its graph [transport plan](../../../../../../transport-plan.md)

$$
\pi_T=(\operatorname{Id},T)_\#\mu.
$$

For [Borel sets](../../../../../../borel-set.md) $A\subseteq X$ and $B\subseteq Y$, the definition of a [pushforward measure](../../../../../../pushforward-measure.md) gives

$$
\pi_T(A\times Y)=\mu(A),\qquad
\pi_T(X\times B)=\mu(T^{-1}(B))=\nu(B).
$$

Hence $\pi_T\in\Pi(\mu,\nu)$. Integration against a [pushforward measure](../../../../../../pushforward-measure.md) also gives

$$
\mathbb K(\pi_T)=\int_X c(x,T(x))\,d\mu(x)=\mathbb M(T).
$$

The [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md) therefore has at least all the competitors of the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md), with exactly the same costs. Consequently

$$
\boxed{\inf_{T_\#\mu=\nu}\mathbb M(T)\ \geq\ \inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi).}
$$

If there is no admissible [transport map](../../../../../../transport-map.md), the left side is $+\infty$ by the convention $\inf\varnothing=+\infty$, so the conclusion still holds. No existence of an optimizer is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
