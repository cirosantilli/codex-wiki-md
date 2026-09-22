<h1 id="9b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual setting of a [continuously differentiable](../../../../../../continuously-differentiable-function.md) [solenoidal vector field](../../../../../../solenoidal-vector-field.md) defined on all radial segments from the origin, including the origin. More generally an open [star-shaped set](../../../../../../star-shaped-set.md) containing zero suffices. [Differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) gives

$$
\nabla\cdot D(x)=\int_0^1t^2(\nabla\cdot B)(tx)\,dt=0.
$$

Apply [divergence and curl of a cross product](../../../../../../divergence-and-curl-of-a-cross-product.md) with the second field $x$, using $\nabla\cdot x=3$ and $(D\cdot\nabla)x=D$:

$$
\nabla\times(D\times x)=3D-x(\nabla\cdot D)+(x\cdot\nabla)D-D
=2D+(x\cdot\nabla)D.
$$

The scaling identity in part (a) now converts the last expression to a one-variable derivative:

$$
2D+(x\cdot\nabla)D
=\int_0^1\left(2tB(tx)+t^2\frac d{dt}B(tx)\right)dt
=\left[t^2B(tx)\right]_0^1=B(x).
$$

Continuity at the origin ensures the lower endpoint is zero. Hence the [radial vector potential of a solenoidal vector field](../../../../../../radial-vector-potential-of-a-solenoidal-vector-field.md) is

$$
\boxed{A(x)=D(x)\times x,\qquad \nabla\times A=B.}
$$

The order of the [cross product](../../../../../../cross-product.md) matters: $x\times D$ would produce $-B$. This construction is not valid on every punctured or multiply connected domain. For example $B=x/|x|^3$ is solenoidal away from zero, but its radial integral diverges at zero and it has nonzero flux through a surrounding [sphere](../../../../../../sphere.md). The stated formula therefore implicitly needs the regular radial-domain hypothesis, rather than just local zero [divergence](../../../../../../divergence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9B](../../9b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
