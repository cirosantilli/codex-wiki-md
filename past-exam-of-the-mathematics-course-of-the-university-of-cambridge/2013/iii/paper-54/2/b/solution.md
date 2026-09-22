<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the horizontal Fourier convention $\widetilde f(\mathbf k)=\int e^{-i\mathbf k\cdot\mathbf R}f(\mathbf R)d^2R$. For each nonzero $k=|\mathbf k|$, the [Poisson equation](../../../../../../poisson-equation.md) becomes

$$
(\partial_z^2-k^2)\widetilde\Phi=4\pi G\widetilde\Sigma\delta(z).
$$

Decay away from the sheet and [continuity](../../../../../../continuous-function.md) at it give $\widetilde\Phi=C e^{-k|z|}$. Its derivative jump is $-2kC=4\pi G\widetilde\Sigma$, hence the [off-plane razor-thin Poisson kernel](../../../../../../off-plane-razor-thin-poisson-kernel.md) is

$$
\boxed{\widetilde\Phi(\mathbf k,z)=-\frac{2\pi G}{k}\widetilde\Sigma(\mathbf k)e^{-k|z|},\qquad
\widetilde\Phi(\mathbf k,\epsilon)=-\frac{2\pi G}{k}\widetilde\Sigma(\mathbf k)e^{-k\epsilon}.}
$$

The spatially uniform mode has a different vertical solution and an arbitrary additive potential reference; it is not obtained by substituting $k=0$ into this decaying-mode formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
