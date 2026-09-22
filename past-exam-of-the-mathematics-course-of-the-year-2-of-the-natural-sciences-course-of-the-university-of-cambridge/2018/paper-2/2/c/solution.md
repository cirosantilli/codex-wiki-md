<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the boundary [Fourier series](../../../../../fourier-series-split.md) as $f=A_0+\sum_{n\geq1}(a_n\cos n\phi+b_n\sin n\phi)$. Since $R=2$, its coefficients obey $a_n=2^nA_n$ and $b_n=2^nB_n$. The mean is

$$
A_0=\frac1{2\pi}\left(\pi+\int_\pi^{2\pi}\cos^2\phi\,d\phi\right)=\frac34.
$$

For $n\geq1$, the integral of $\cos n\phi$ on the first semicircle is zero. On the second semicircle, use $\cos^2\phi=(1+\cos2\phi)/2$ and [cosine](../../../../../cosine.md) [orthogonality](../../../../../orthogonal-vectors.md). This gives $a_2=1/4$ and every other $a_n=0$.

For the [sine](../../../../../sine.md) coefficients, every even $n$ gives zero on both semicircles. For odd $n$, [product-to-sum formulas](../../../../../product-to-sum-formula.md) give

$$
\begin{aligned}
\pi b_n&=\int_0^\pi\sin n\phi\,d\phi+
\int_\pi^{2\pi}\frac{1+\cos2\phi}{2}\sin n\phi\,d\phi\\
&=\frac2n-\frac1n-\frac12\left(\frac1{n+2}+\frac1{n-2}\right)
=\frac{4}{n(4-n^2)}.
\end{aligned}
$$

Thus the requested radial-expansion coefficients are

$$
\boxed{A_0=\frac34,\qquad A_n=\begin{cases}1/16,&n=2,\\0,&n\ne2,\end{cases}\qquad
B_n=\begin{cases}\displaystyle\frac{4}{\pi\,2^n n(4-n^2)},&n\text{ odd},\\0,&n\text{ even}.\end{cases}}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
