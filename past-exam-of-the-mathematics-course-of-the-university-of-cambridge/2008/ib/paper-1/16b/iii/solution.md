<h1 id="16b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the identity $\nabla\times\mathbf B=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A$. The [Laplacian](../../../../../../laplacian.md) identity for the Coulomb [kernel](../../../../../../kernel-of-a-linear-map.md) gives, component by component,

$$
-\nabla^2\mathbf A=-\frac{\mu_0}{4\pi}\int\mathbf J(\mathbf r')\nabla^2(s^{-1})\,dV'=\mu_0\mathbf J(\mathbf r).
$$

Also $\nabla(s^{-1})=-\nabla'(s^{-1})$, so [integration by parts](../../../../../../integration-by-parts.md) yields

$$
\begin{aligned}\nabla\cdot\mathbf A&=-\frac{\mu_0}{4\pi}\int\mathbf J(\mathbf r')\cdot\nabla'(s^{-1})\,dV'\\&=\frac{\mu_0}{4\pi}\int\frac{\nabla'\cdot\mathbf J(\mathbf r')}{s}\,dV'.\end{aligned}
$$

Here the surface integral at infinity vanishes under the assumed localization of the current. As usual, this assumption means sufficient decay for these integrals and the boundary limit, rather than merely pointwise convergence to zero. Combining the two terms gives

$$
\boxed{\nabla\times\mathbf B=\mu_0\mathbf J+\frac{\mu_0}{4\pi}\nabla\int\frac{\nabla'\cdot\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,dV'.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [16B](../../16b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
