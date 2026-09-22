<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The flat four-dimensional [retarded Green function](../../../../../../../retarded-green-function.md) is

$$
G_{\rm ret}^{(4)}(t,\mathbf X)
=\frac{\theta(t)}{2\pi}
\delta(t^2-|\mathbf X|^2).
$$

For a [Dirichlet boundary condition](../../../../../../../dirichlet-boundary-condition.md) at $z=0$, the [method of images](../../../../../../../method-of-images.md) gives

$$
G_D(X;X')=G_{\rm ret}^{(4)}(x-x',z-z')
-G_{\rm ret}^{(4)}(x-x',z+z').
$$

The boundary-to-bulk kernel for $\psi$ is its inward boundary derivative. For a source at the spacetime origin,

$$
G_\psi(x,z|0)
=\left.\partial_{z'}G_D(x,z;0,z')\right|_{z'=0}
=\frac{2z}{\pi}\theta(t)
\delta'\left(t^2-x^2-y^2-z^2\right).
$$

Multiplying by the Weyl factor $z$ gives the requested kernel for the original bulk field:

$$
\boxed{G(x,z|0)
=\frac{2z^2}{\pi}\theta(t)
\delta'\left(t^2-x^2-y^2-z^2\right)}.
$$

It is causal and supported on the future bulk light cone of the boundary insertion. Its distributional boundary limit satisfies $\phi/z\to\delta^3(x)$, while the source-free initial term vanishes for the CFT vacuum in this response calculation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 354](../../../../paper-354-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
