<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The direct squared [L2 norm](../../../../../l2-norm.md) is the length of the interval, namely $2$. The [Fourier transform](../../../../../fourier-transform-split.md) is

$$
\widehat f(k)=\int_{-1}^1e^{-ikx}dx=\frac{2\sin k}{k},\qquad \widehat f(0)=2.
$$

For the transformed norm, let $I=\int_0^\infty\sin^2k/k^2\,dk$. [Integration by parts](../../../../../integration-by-parts.md), with vanishing endpoint term $-\sin^2k/k$, gives

$$
I=2\int_0^\infty\frac{\sin k\cos k}{k}\,dk=\frac\pi2.
$$

The supplied oscillatory integral is understood as an [improper integral](../../../../../improper-integral.md). Therefore

$$
\boxed{\frac1{2\pi}\int_{-\infty}^{\infty}\left|\frac{2\sin k}{k}\right|^2dk=\frac4\pi I=2,}
$$

which agrees with the direct norm and verifies the [Parseval identity](../../../../../parseval-identity.md) with the specified normalization.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
