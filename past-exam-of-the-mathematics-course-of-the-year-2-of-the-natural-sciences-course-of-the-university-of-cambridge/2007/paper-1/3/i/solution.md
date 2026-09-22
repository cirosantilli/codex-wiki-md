<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extend $f$ evenly to $F(x)=f(|x|)$ on the whole real line, and use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widehat F(k)=\int_{\mathbb R}F(x)e^{-ikx}dx$. Its odd sine contribution vanishes, giving $\widehat F(k)=2\int_0^\infty f(x)\cos(kx)dx=\widehat f_c(k)$ for $k>0$; the transform is also [even](../../../../../even-function.md). The [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) therefore gives, for $x>0$,

$$
f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}\widehat F(k)e^{ikx}dk=\boxed{\frac1\pi\int_0^\infty\widehat f_c(k)\cos(kx)dk}.
$$

This is the inverse [Fourier cosine transform](../../../../../fourier-cosine-transform.md) with the factor-of-two forward convention used here.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
