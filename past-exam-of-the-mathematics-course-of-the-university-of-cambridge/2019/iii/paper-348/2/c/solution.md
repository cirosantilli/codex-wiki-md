<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every admissible [transport map](../../../../../../transport-map.md) $T$, the [pushforward measure](../../../../../../pushforward-measure.md) condition gives $T(x)\in[1,2]$ for $\mu$-almost every $x\in[0,1]$. Hence $|T(x)-x|=T(x)-x$, and

$$
\int_0^1(T(x)-x)\,dx
=\int_1^2 y\,dy-\int_0^1x\,dx=1.
$$

Apply the [Jensen inequality](../../../../../../jensen-s-inequality.md) to the [convex function](../../../../../../convex-function.md) $h$ and the [probability measure](../../../../../../probability-measure.md) $\mu$:

$$
\mathbb M(T)=\int_0^1h(T(x)-x)\,dx\geq h\left(\int_0^1(T(x)-x)\,dx\right)=h(1).
$$

Translation by one sends the source [uniform distribution](../../../../../../continuous-uniform-distribution.md) to the target [uniform distribution](../../../../../../continuous-uniform-distribution.md), so $T^\dagger(x)=x+1$ is admissible. Its displacement is constantly one, giving

$$
\boxed{T^\dagger(x)=x+1,\qquad\min_{T_\#\mu=\nu}\mathbb M(T)=h(1).}
$$

No monotonicity assumption on $h$ is needed, because all displacements have the same sign. The same argument with a [transport plan](../../../../../../transport-plan.md) also gives the identical minimum for the [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
