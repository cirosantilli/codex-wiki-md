<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\mathbf F=\mathbf r\,r^{-\gamma-1}$. For $r>0$, direct Cartesian differentiation gives the [divergence and curl of a radial vector field](../../../../divergence-and-curl-of-a-radial-vector-field.md):

$$
\partial_i(x_i r^{-\gamma-1})=3r^{-\gamma-1}-(\gamma+1)r^{-\gamma-3}x_ix_i=(2-\gamma)r^{-\gamma-1}.
$$

The volume element in [spherical coordinates](../../../../spherical-coordinate-system.md) therefore gives, for $\gamma\ne2$,

$$
\boxed{\int_V\nabla\cdot\mathbf F\,dV=4\pi(2-\gamma)\int_\epsilon^R r^{1-\gamma}dr=4\pi(R^{2-\gamma}-\epsilon^{2-\gamma}).}
$$

For the direct [surface integral](../../../../surface-integral.md), the outer sphere has outward normal $+\mathbf n$ and contributes $4\pi R^{2-\gamma}$. The inner boundary's outward normal relative to the shell is $-\mathbf n$, so it contributes $-4\pi\epsilon^{2-\gamma}$. Hence

$$
\boxed{\int_S\mathbf F\cdot d\mathbf A=4\pi(R^{2-\gamma}-\epsilon^{2-\gamma}).}
$$

For $\gamma=2$, the field has zero ordinary divergence everywhere in this shell. The separate surface contributions are $4\pi$ and $-4\pi$, so **both full integrals are zero**. This [radial power-law flux through a spherical shell](../../../../radial-power-law-flux-through-a-spherical-shell.md) was obtained by direct differentiation and integration; the excluded origin is never part of the volume.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
