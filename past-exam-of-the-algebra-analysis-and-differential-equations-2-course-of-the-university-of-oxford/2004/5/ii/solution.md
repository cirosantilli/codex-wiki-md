<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a nonnegative [integer](../../../../integer-split.md) $n$, put $z=e^{i\theta}$ on the [unit circle](../../../../complex-unit-circle.md). Since $\cos\theta=(z+z^{-1})/2$ and $d\theta=dz/(iz)$,

$$
\int_0^{2\pi}\cos^{2n}\theta\,d\theta
=\frac1{i4^n}\int_{|z|=1}\frac{(z^2+1)^{2n}}{z^{2n+1}}\,dz.
$$

The [residue](../../../../residue.md) at zero is the coefficient of $z^{2n}$ in $(1+z^2)^{2n}$, namely $\binom{2n}{n}$. The [residue theorem](../../../../residue-theorem.md) gives

$$
\boxed{\int_0^{2\pi}\cos^{2n}\theta\,d\theta
=\frac{2\pi}{4^n}\binom{2n}{n}.}
$$

The contour integrand has no other [poles](../../../../pole.md). The formula also includes $n=0$, giving $2\pi$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
