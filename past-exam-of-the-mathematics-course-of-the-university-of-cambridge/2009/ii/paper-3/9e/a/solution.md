<h1 id="9e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put the cylinder's centre at the origin, with $-h/2\le z\le h/2$, $0\le r\le a$, and uniform density $\rho=M/(\pi a^2h)$. Symmetry makes the [inertia tensor](../../../../../../inertia-tensor.md) diagonal and gives $I_1=I_2$. Direct integration yields

$$
I_3=\rho\int_{-h/2}^{h/2}\!dz\int_0^a\!r^3dr\int_0^{2\pi}\!d\theta=\frac{Ma^2}{2}.
$$

For a transverse [principal moment of inertia](../../../../../../principal-moment-of-inertia.md), the two contributions are

$$
\int y^2\,dm=\rho h\frac{a^4}{4}\int_0^{2\pi}\sin^2\theta\,d\theta=\frac{Ma^2}{4},\qquad
\int z^2\,dm=\rho\pi a^2\frac{h^3}{12}=\frac{Mh^2}{12}.
$$

Therefore $\boxed{I_1=I_2=M(a^2/4+h^2/12),\quad I_3=Ma^2/2}$ are the three [principal moments of inertia](../../../../../../principal-moment-of-inertia.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9E](../../9e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
