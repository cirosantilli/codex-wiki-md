<h1 id="29c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [Fourier series](../../../../../../fourier-series-split.md) $f(x)=\sum_{n\in\mathbb Z}f_ne^{inx}$, with $f_n=(2\pi)^{-1}\int_{-\pi}^{\pi}f(x)e^{-inx}\,dx$. Smoothness makes its coefficients decay faster than every inverse power. Setting

$$
\boxed{u_f(x)=\sum_{n\in\mathbb Z}\frac{f_n}{1+n^2}e^{inx}}
$$

therefore gives a smooth periodic function, and termwise differentiation proves $-u_f''+u_f=f$. Conversely every solution must have these coefficients, proving uniqueness. Equivalently, a homogeneous solution has $\int(|u'|^2+|u|^2)=0$ by [integration by parts](../../../../../../integration-by-parts.md), so vanishes.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [29C](../../29c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
