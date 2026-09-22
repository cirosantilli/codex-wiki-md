<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With the stated angular-frequency convention, the [inverse Fourier transform](../../../../inverse-fourier-transform.md) is $f(x)=(2\pi)^{-1}\int_{-\infty}^{\infty}\widetilde f(k)e^{ikx}dk$. Direct integration gives $\widetilde f_0(k)=\int_0^\infty e^{-(\alpha+ik)x}dx=1/(\alpha+ik)$. For $n\geq1$, [integration by parts](../../../../integration-by-parts.md) has zero boundary terms and gives $\widetilde f_n=n\widetilde f_{n-1}/(\alpha+ik)$. Therefore

$$
\boxed{\widetilde f_n(k)=\frac{n!}{(\alpha+ik)^{n+1}}.}
$$

This also follows from the [Fourier transform of a polynomial multiple](../../../../fourier-transform-of-a-polynomial-multiple.md), since multiplication by $x$ corresponds to $i\partial_k$.

To prove [Parseval's identity](../../../../parseval-identity.md), substitute the inverse transform of $g$ into $\int f^*g$. Under the assumed integrability, [Fubini's theorem](../../../../fubini-s-theorem.md) permits interchange, and the inner integral is $\int f(x)^*e^{ikx}dx=\widetilde f(k)^*$. Hence

$$
\int_{\mathbb R}f(x)^*g(x)dx=\frac1{2\pi}\int_{\mathbb R}\widetilde f(k)^*\widetilde g(k)dk.
$$

Apply this with $f=g=f_n$. The spatial [Gamma integral](../../../../gamma-integral.md) is $\int_0^\infty x^{2n}e^{-2\alpha x}dx=(2n)!/(2\alpha)^{2n+1}$. The transformed squared modulus is $(n!)^2/(\alpha^2+k^2)^{n+1}$, giving the scaled [even rational Parseval integral](../../../../even-rational-parseval-integral.md)

$$
\boxed{\int_{-\infty}^{\infty}\frac{dk}{(\alpha^2+k^2)^{n+1}}=\frac{2\pi(2n)!}{(n!)^2(2\alpha)^{2n+1}}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
