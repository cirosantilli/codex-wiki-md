<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A map $g$ is [differentiable](../../../../differentiable-function.md) at $a$ when a [linear map](../../../../linear-map.md) $Dg_a:\mathbb R^n\to\mathbb R^k$ approximates its increment to first order:

$$
\boxed{g(a+h)=g(a)+Dg_a(h)+o(\|h\|).}
$$

This [Fréchet derivative](../../../../frechet-derivative.md) is unique, and its matrix in the standard bases is the [Jacobian matrix](../../../../jacobian-matrix.md). Differentiability on a domain means differentiability at each point there.

A standard sufficient condition for a zero locus to be a [submanifold](../../../../submanifold.md) is the [regular level set theorem](../../../../regular-level-set-theorem.md): if $g$ is $C^1$ on an open domain and $Dg_a$ is [surjective](../../../../surjective-function.md) at every $a\in g^{-1}(0)$, then

$$
\boxed{M=g^{-1}(0)\text{ is an embedded }C^1\text{ submanifold of dimension }n-k.}
$$

For smooth $g$, the [submanifold](../../../../submanifold.md) is smooth. The full-rank condition is the relevant [constraint qualification](../../../../constraint-qualification.md).

Under this regularity hypothesis, its [tangent space](../../../../tangent-space.md) is

$$
\boxed{T_aM=\ker Dg_a.}
$$

Indeed, if a differentiable curve $\gamma$ lies in $M$ and passes through $a$, the [chain rule](../../../../chain-rule.md) gives $Dg_a(\gamma'(0))=0$. Thus all tangent velocities lie in the [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md). The [rank-nullity theorem](../../../../rank-nullity-theorem.md) makes this kernel $(n-k)$-dimensional, the same dimension as the [tangent space](../../../../tangent-space.md), proving equality. In coordinates, solve the homogeneous linear equations given by the [Jacobian matrix](../../../../jacobian-matrix.md).

The regularity qualification matters: $g(x)=x^2$ has zero set $\{0\}$, a zero-dimensional [submanifold](../../../../submanifold.md), but $Dg_0=0$. Its [kernel](../../../../kernel-of-a-linear-map-split.md) is all of $\mathbb R$, whereas its [tangent space](../../../../tangent-space.md) is zero. This is the phenomenon that [singular defining maps can overestimate tangent spaces](../../../../singular-defining-maps-can-overestimate-tangent-spaces.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
