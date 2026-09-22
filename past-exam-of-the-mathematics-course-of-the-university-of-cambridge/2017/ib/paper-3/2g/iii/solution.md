<h1 id="2g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $x_n=(\pi/2+2\pi n)^{-1}$. The points $p_n=(x_n,1)$ lie on the specified graph and converge in $\mathbb R^2$ to $(0,1)$. They form a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the induced [metric](../../../../../../metric.md), but their only possible limit is absent from the space. Adding $(0,0)$ does not supply that missing limit. Hence the specified space is **not complete**.

For the unheaded request on $\mathbb R$, use the [arctangent pullback metric](../../../../../../arctangent-pullback-metric.md)

$$
\boxed{d(x,y)=|\arctan x-\arctan y|.}
$$

Positivity, symmetry and the [triangle inequality](../../../../../../triangle-inequality.md) follow from the ordinary distance, and injectivity of $\arctan$ gives $d(x,y)=0$ only if $x=y$. The sequence $n$ is Cauchy for this [metric](../../../../../../metric.md), because $\arctan n\to\pi/2$, but cannot converge to any finite real $x$: that would require $\arctan x=\pi/2$. Thus this [metric](../../../../../../metric.md) makes $\mathbb R$ incomplete, even though it induces its usual topology.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2G](../../2g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
