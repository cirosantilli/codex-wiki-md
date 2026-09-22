<h1 id="4/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $z=e^{i\theta}$, so $\sin\theta=(z-z^{-1})/(2i)$ and $d\theta=dz/(iz)$. The [unit circle](../../../../../../complex-unit-circle.md) is traversed anticlockwise, and the integral becomes

$$
\oint_{|z|=1}\frac{2\,dz}{-3z^2+10iz+3}
=\oint_{|z|=1}\frac{2\,dz}{-3(z-i/3)(z-3i)}.
$$

Only the [simple pole](../../../../../../simple-pole.md) $z=i/3$ lies inside the [contour](../../../../../../complex-integration-contour.md). Its [residue](../../../../../../residue.md) is

$$
\frac{2}{-6(i/3)+10i}=\frac1{4i}.
$$

Hence the [residue theorem](../../../../../../residue-theorem.md) gives

$$
\boxed{\int_0^{2\pi}\frac{d\theta}{5-3\sin\theta}=2\pi i\frac1{4i}=\frac\pi2}.
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
