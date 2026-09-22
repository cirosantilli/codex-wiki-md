<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

The [implicit function theorem](../../../../../implicit-function-theorem.md) states that if $F(x_0,y_0)=0$ and the partial derivative $D_yF(x_0,y_0)$ is an [invertible linear map](../../../../../invertible-linear-map.md), then near $(x_0,y_0)$ the zero set of $F$ is uniquely the graph $y=g(x)$ of a continuously differentiable function.

If $f$ is a [differentiable](../../../../../differentiable-map.md) bijection with differentiable inverse $g$, the [chain rule](../../../../../chain-rule.md) applied to $g\circ f$ and $f\circ g$ gives

$$
Dg_{f(x)}Df_x=I,
\qquad
Df_xDg_{f(x)}=I.
$$

Thus $Df_x$ is an isomorphism with inverse $Dg_{f(x)}$.

If a continuously differentiable map $F:\mathbb R^n\to\mathbb R^n$ has invertible derivative everywhere, the [inverse function theorem](../../../../../inverse-function-theorem.md) makes it a local diffeomorphism. In particular it is an [open map](../../../../../open-map.md), so its image is open. Its image need not be closed: $x\mapsto\arctan x$ has nonzero derivative everywhere and image $(-\pi/2,\pi/2)$.

For the given map of [elementary symmetric polynomials](../../../../../elementary-symmetric-polynomial.md),

$$
DF=
\begin{pmatrix}
1&1&1\\
y+z&x+z&x+y\\
yz&xz&xy
\end{pmatrix},
$$

and direct evaluation of the [determinant](../../../../../determinant.md) gives

$$
\det DF=(x-y)(y-z)(z-x).
$$

Hence the [critical set](../../../../../critical-set.md) is

$$
\boxed{C=\{x=y\}\cup\{y=z\}\cup\{z=x\}}.
$$

Its complement is the [Zariski-open set](../../../../../zariski-open-set.md) on which the three coordinates are pairwise distinct. Each point has one of the six possible strict coordinate orderings, and each ordering defines a nonempty convex open region. A [continuous path](../../../../../continuous-path.md) cannot change an ordering without crossing $C$. Therefore $\mathbb R^3\setminus C$ has exactly

$$
\boxed{3!=6}
$$

[connected components](../../../../../connected-component.md).

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
