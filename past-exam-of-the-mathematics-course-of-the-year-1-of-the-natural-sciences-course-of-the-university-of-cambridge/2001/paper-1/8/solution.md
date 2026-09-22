<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Write $r=|\mathbf r|$ and $q=\mathbf p\cdot\mathbf r$. Away from the origin, $\nabla q=\mathbf p$ and $\nabla r^{-m}=-m\mathbf r/r^{m+2}$. The [product rule](../../../../product-rule.md) gives

$$
\nabla\cdot(q\mathbf r r^{-5})=q r^{-5}+q(3r^{-5}-5r^{-5})=-q r^{-5},\qquad \nabla\cdot(\mathbf p r^{-3})=-3q r^{-5}.
$$

Consequently the [divergence](../../../../divergence.md) of $\mathbf E=3q\mathbf r r^{-5}-\mathbf p r^{-3}$ is zero. For any closed surface bounding a region that excludes the origin, the field is smooth throughout that region, and the [divergence theorem](../../../../divergence-theorem.md) proves

$$
\boxed{\int_A\mathbf E\cdot d\mathbf S=0.}
$$

For the infinite cylinder, use $\mathbf r=(a\cos\phi,a\sin\phi,z)$ and outward [unit normal](../../../../unit-normal.md) $(\cos\phi,\sin\phi,0)$. With $\mathbf p=(0,0,1)$, $q=z$, $dS=a\,d\phi\,dz$, and $\mathbf E\cdot\mathbf n=3az/(a^2+z^2)^{5/2}$. Hence the direct [surface flux](../../../../flux-integral.md) is

$$
\int_0^{2\pi}\int_{-\infty}^\infty\frac{3a^2z}{(a^2+z^2)^{5/2}}dz\,d\phi=\boxed0.
$$

The integrand is [odd](../../../../odd-function.md) in $z$ and absolutely integrable. This calculation treats the unbounded cylindrical side directly, without applying the bounded-region [divergence theorem](../../../../divergence-theorem.md) across the field's singularity.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
