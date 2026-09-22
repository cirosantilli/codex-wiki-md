<h1 id="11/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [gradient](../../../../../../gradient.md) part contributes zero around a closed path by the [fundamental theorem for line integrals](../../../../../../fundamental-theorem-for-line-integrals.md):

$$
\oint_{\Gamma_1}3\nabla\phi\cdot d\mathbf x=0.
$$

Along the parametrization, $x^2+z^2=1$, so the first two components of $\mathbf w$ vanish wherever the printed expression is defined. The remaining component gives $\mathbf w\cdot d\mathbf x=x\,dz=\cos^2\theta\,d\theta$. Thus

$$
\boxed{\oint_{\Gamma_1}(3\mathbf v+\mathbf w)\cdot d\mathbf x
=\int_0^{2\pi}\cos^2\theta\,d\theta=\pi}.
$$

**The printed field needs a qualification:** $\operatorname{arctanh}(x^2)$ is undefined at the isolated parameters where $x^2=1$, so $0\operatorname{arctanh}(1)$ cannot literally be evaluated. The result above is the [improper line integral](../../../../../../improper-line-integral.md), or equivalently the [integral](../../../../../../integral-split.md) of the continuous extension of the restricted field along the [curve](../../../../../../curve.md). That restricted field tends to $(0,0,\cos\theta)$ at each omitted parameter. No extension of the full field to a neighbourhood is being assumed.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [11](../../../11.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
