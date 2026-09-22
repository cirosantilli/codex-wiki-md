<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the open strip $S=\{x+iy:0<y<\pi\}$; the printed closed strip denotes the region together with its exit boundary. Starting at $z=x+iy$, the [conformal bijection](../../../../../../biholomorphism.md) $e^z$ sends $S$ onto the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) and the bottom edge $a\in\mathbb R$ onto $v=e^a>0$. The upper edge maps to the negative half-axis. The transformed initial point is $e^x\cos y+i e^x\sin y$.

By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md), transform the given [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) and include the [Jacobian determinant](../../../../../../jacobian-determinant.md) $dv/da=e^a$. The **[bottom-boundary harmonic measure of a strip](../../../../../../bottom-boundary-harmonic-measure-of-a-strip.md)** is

$$
\boxed{\rho_z(a)=\frac{e^{a+x}\sin y}{\pi\bigl((e^a-e^x\cos y)^2+e^{2x}\sin^2y\bigr)}=\frac{\sin y}{2\pi\bigl(\cosh(a-x)-\cos y\bigr)}.}
$$

This is the unconditional exit density on the bottom edge, not the density conditional on using that edge. Its total mass is

$$
\boxed{\int_{\mathbb R}\rho_z(a)da=1-\frac y\pi.}
$$

Indeed substitution $v=e^{a-x}$ gives the positive-half-axis mass of the [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md), equal to $\frac12+\pi^{-1}\arctan(\cot y)=1-y/\pi$ for $0<y<\pi$. To obtain the conditional bottom-edge density, divide by $1-y/\pi$. The top-edge density is $\sin y/[2\pi(\cosh(a-x)+\cos y)]$ and has mass $y/\pi$, a useful normalization check.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
