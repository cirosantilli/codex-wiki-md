<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

As in part (c), every admissible [transport map](../../../../../../transport-map.md) has nonnegative displacement $D(x)=T(x)-x$ with $\int_0^1D(x)\,dx=1$. The square root is a [strictly concave function](../../../../../../strictly-concave-function.md), so the reversed [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
\mathbb M(T)=\int_0^1\sqrt{D(x)}\,dx\leq\sqrt{\int_0^1D(x)\,dx}=1.
$$

The map $T^\dagger(x)=x+1$ is admissible and attains one. Therefore

$$
\boxed{\max_{T_\#\mu=\nu}\mathbb M(T)=1,\qquad T^\dagger(x)=x+1.}
$$

Thus “worst” means largest cost among admissible [transport maps](../../../../../../transport-map.md). Equality in the [Jensen inequality](../../../../../../jensen-s-inequality.md) for a [strictly concave function](../../../../../../strictly-concave-function.md) forces $D(x)$ to be constant almost everywhere, so this maximizer is unique up to a $\mu$-null set. For comparison, the admissible reflection $T(x)=2-x$ has smaller cost

$$
\int_0^1\sqrt{2-2x}\,dx=\frac{2\sqrt2}{3}<1.
$$

The upper bound also holds for every [transport plan](../../../../../../transport-plan.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
