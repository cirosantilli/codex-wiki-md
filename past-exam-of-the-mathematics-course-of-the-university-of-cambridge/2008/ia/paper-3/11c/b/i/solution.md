<h1 id="11c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $v=z$, so $\nabla v=\mathbf e_z$, while $\nabla u=\widehat{\mathbf r}$ away from the origin. Their [inner product](../../../../../../../inner-product.md) is $\cos\theta$. The [spherical coordinates](../../../../../../../spherical-coordinate-system.md) volume element gives

$$
\int_V\nabla u\cdot\nabla v\,dV=\int_0^a r^2\,dr\int_0^\pi\cos\theta\sin\theta\,d\theta\int_0^{2\pi}d\varphi=\boxed{0}.
$$

This agrees with the boundary-constant [gradient pairing with a boundary-constant function and a harmonic function](../../../../../../../gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function.md): $u$ has constant boundary value $a$ and $v=z$ is a regular [harmonic function](../../../../../../../harmonic-function.md). For comparison with the boundary value one in part (a), use $u/a$ and multiply back by $a$. Strictly, $u=r$ is not differentiable at the origin. Excising a ball of radius $\varepsilon$ resolves this: the inner boundary term $u\partial_n v=-\varepsilon\cos\theta$ has zero angular integral, so it contributes nothing in the limit. Thus the improper [volume integral](../../../../../../../volume-integral.md) has the same zero value.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [11C](../../../11c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
