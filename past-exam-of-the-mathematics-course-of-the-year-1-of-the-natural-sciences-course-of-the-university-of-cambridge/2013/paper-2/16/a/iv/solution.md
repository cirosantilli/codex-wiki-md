<h1 id="16/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $R=\sqrt8$ and parametrize the circle counterclockwise, as viewed from positive $z$, by $\mathbf r(\phi)=(R\cos\phi,R\sin\phi,3)$ for $0\leq\phi\leq2\pi$. The restricted field is

$$
V(\phi)=2R^3\cos^3\phi+R^2\sin^2\phi+27-R\sin\phi.
$$

**The PDF does not specify the differential in this [line integral](../../../../../../line-integral.md).** An oriented [vector line integral weighted by a scalar field](../../../../../../vector-line-integral-weighted-by-a-scalar-field.md) uses $d\mathbf r=(-R\sin\phi,R\cos\phi,0)\,d\phi$. Its two nonzero components are

$$
\begin{aligned}
\oint_\Gamma V\,dx&=-R\int_0^{2\pi}V(\phi)\sin\phi\,d\phi=\pi R^2,\\
\oint_\Gamma V\,dy&=R\int_0^{2\pi}V(\phi)\cos\phi\,d\phi
=2R^4\int_0^{2\pi}\cos^4\phi\,d\phi=\frac32\pi R^4.
\end{aligned}
$$

All other terms vanish by sine-cosine symmetry. Thus this interpretation gives

$$
\boxed{\oint_\Gamma V\,d\mathbf r=(8\pi,96\pi,0)}.
$$

If the intended convention is the scalar [arc length](../../../../../../arc-length.md) [integral](../../../../../../integral-split.md), then $ds=R\,d\phi$ and

$$
\oint_\Gamma V\,ds=R\left(R^2\int_0^{2\pi}\sin^2\phi\,d\phi+54\pi\right)
=\boxed{124\sqrt2\,\pi}.
$$

That scalar [integral](../../../../../../integral-split.md) is independent of traversal direction. Giving both values retains the actual distinction left unspecified by the wording.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [16](../../../16.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
