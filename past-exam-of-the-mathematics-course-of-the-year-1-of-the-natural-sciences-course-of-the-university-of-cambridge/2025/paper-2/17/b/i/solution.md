<h1 id="17/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the two pieces of the [surface integral](../../../../../../surface-integral.md) directly; this avoids introducing an unnecessary second [derivative](../../../../../../derivative.md) of $f$. On the unit [sphere](../../../../../../sphere.md), $\mathbf n=\mathbf r$ and $\mathbf F\cdot\mathbf n=f'(z)$. A spherical band between heights $z$ and $z+dz$ has [area](../../../../../../surface-area.md) $2\pi\,dz$, so the curved [flux](../../../../../../flux.md) is

$$
\Phi_{\mathrm{curved}}=2\pi\int_{-1}^{z_0}f'(z)\,dz
=2\pi\bigl(f(z_0)-f(-1)\bigr),
$$

by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md). On the horizontal top [disk](../../../../../../disk-mathematics.md), $\mathbf F\cdot\mathbf n=z_0f'(z_0)$ and the [area](../../../../../../surface-area.md) is $\pi(1-z_0^2)$. Thus

$$
\boxed{\Phi(z_0)=2\pi\bigl(f(z_0)-f(-1)\bigr)
+\pi z_0(1-z_0^2)f'(z_0)}.
$$

As usual for these [surface integrals](../../../../../../surface-integral.md), the first [derivative](../../../../../../derivative.md) is assumed sufficiently integrable for the displayed [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) evaluation; a continuous first [derivative](../../../../../../derivative.md) suffices. Mere pointwise [differentiability](../../../../../../differentiability.md) without such an integrability assumption need not make an ordinary [flux integral](../../../../../../flux-integral.md) exist.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [17](../../../17.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
