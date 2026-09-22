<h1 id="8c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) on the moving drop:

$$
\frac{dM}{dt}=R\,h(R,t)\dot R+\int_0^Rrh_t\,dr
=\left[rh^3h_r\right]_0^R.
$$

The moving-boundary term vanishes because $h(R,t)=0$. At the origin, symmetry and regularity give $h_r(0,t)=0$. At the front, the stated $h\propto(R-r)^{1/3}$ gives $h^3h_r=O((R-r)^{1/3})\to0$. Thus $\boxed{dM/dt=0}$, expressing [volume conservation](../../../../../../volume-conservation.md) for this [axisymmetric viscous gravity current](../../../../../../axisymmetric-viscous-gravity-current.md).

With $\eta=r/t^\alpha$ and $R=\eta_0t^\alpha$, substitute the [self-similar solution](../../../../../../similarity-solution.md) into the conserved integral:

$$
M=t^{2\alpha-1/4}\int_0^{\eta_0}\eta f(\eta)\,d\eta.
$$

For a nonzero finite drop volume, the power of $t$ must vanish, so $\boxed{\alpha=1/8}$. Balancing powers in the evolution equation gives the same result: its left side scales as $t^{-5/4}$ and its right side as $t^{-1-2\alpha}$. The front-edge exponent alone would not determine this spreading exponent without the conserved volume.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8C](../../8c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
