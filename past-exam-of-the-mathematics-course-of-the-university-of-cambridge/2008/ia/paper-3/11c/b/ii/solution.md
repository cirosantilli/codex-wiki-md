<h1 id="11c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Now $v=z^2$ and $\nabla v=2z\mathbf e_z$. Since $\nabla u=\widehat{\mathbf r}/a$, their [inner product](../../../../../../../inner-product.md) is $2r\cos^2\theta/a$. Consequently

$$
\int_V\nabla u\cdot\nabla v\,dV=\frac2a\int_0^a r^3\,dr\int_0^\pi\cos^2\theta\sin\theta\,d\theta\int_0^{2\pi}d\varphi
=\frac2a\frac{a^4}{4}\frac23(2\pi)=\boxed{\frac{2\pi a^3}{3}}.
$$

Although $u=1$ on the boundary, the [Laplacian](../../../../../../../laplacian.md) is $\nabla^2v=2$, so $v$ is not a [harmonic function](../../../../../../../harmonic-function.md). There is no contradiction with part (a). The origin singularity in the derivative of $u$ is harmless for this integral: its inner boundary contribution is of order $\varepsilon^4/a$ and tends to zero. More explicitly, [Green's first identity](../../../../../../../green-s-first-identity.md) on the punctured ball gives outer flux $8\pi a^3/3$ and volume term $\int_V2r/a\,dV=2\pi a^3$, whose difference is the displayed answer.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
