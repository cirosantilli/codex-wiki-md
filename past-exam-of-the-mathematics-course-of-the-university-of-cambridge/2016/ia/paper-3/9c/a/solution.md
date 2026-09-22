<h1 id="9c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [conservative vector field](../../../../../../conservative-vector-field.md) on $\mathbb R^n$ is a [vector field](../../../../../../vector-field.md) $\mathbf V=\nabla F$ for a globally defined smooth [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md) $F$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\int_C\mathbf V\cdot d\mathbf x=F(\text{endpoint})-F(\text{startpoint}),
$$

so its [line integral](../../../../../../line-integral.md) is [path independent](../../../../../../path-independence.md).

[Green theorem](../../../../../../green-theorem.md) states that, for a bounded planar region $D$ with piecewise smooth boundary and continuously differentiable $P,Q$ on a neighbourhood of its closure,

$$
\boxed{\oint_{\partial D}(P\,dx+Q\,dy)=\iint_D(Q_x-P_y)\,dx\,dy.}
$$

The boundary is positively oriented: the region lies on the left while it is traversed, so outer components run counterclockwise and hole boundaries clockwise.

For the proposed [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md), the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) and [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) give

$$
F_y(x,y)=Q(x,y),\qquad F_x(x,y)=P(x,0)+\int_0^yQ_x(x,s)\,ds.
$$

Since $Q_x=P_y$, the last integral equals $P(x,y)-P(x,0)$, including negative $y$ with the usual signed-integral convention. Hence **the proposed potential is global and**

$$
\boxed{\nabla F=(P,Q)=\mathbf V.}
$$

The fact that the [vector field](../../../../../../vector-field.md) is defined on all of $\mathbb R^2$ ensures both straight integration segments stay inside its domain; a hole in the domain could obstruct a global potential.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9C](../../9c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
