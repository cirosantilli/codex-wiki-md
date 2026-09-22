<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Using the normalized [eigenfunctions](../../../../../../eigenfunction.md) and the same change of variables, their [weighted inner product](../../../../../../weighted-inner-product.md) is

$$
\int_{-1}^1\frac{y_m(x)y_n(x)}{\sqrt{1-x^2}}\,dx=\frac2\pi\int_0^\pi\sin(m\theta)\sin(n\theta)\,d\theta.
$$

For distinct positive integers $m,n$, the product-to-sum identity gives

$$
\frac1\pi\int_0^\pi[\cos((m-n)\theta)-\cos((m+n)\theta)]d\theta=0,
$$

because each integrated sine has integer-multiple-of-$\pi$ endpoints. For $m=n$, the integral is one by the normalization already calculated. Hence

$$
\boxed{\int_{-1}^1w(x)y_m(x)y_n(x)\,dx=\delta_{mn}.}
$$

This verifies [orthonormality](../../../../../../orthonormal-set.md) explicitly, with $\delta_{mn}$ the [Kronecker delta](../../../../../../kronecker-delta.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
