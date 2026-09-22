<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [integration by parts](../../../../../integration-by-parts.md) in $I_{n+1}$, writing the integrand as $x^{2n+1}(xe^{-x^2})$. Since an [antiderivative](../../../../../antiderivative.md) of $xe^{-x^2}$ is $-e^{-x^2}/2$,

$$
\begin{aligned}
I_{n+1}
&=\left[-\frac12x^{2n+1}e^{-x^2}\right]_{-\infty}^{\infty}
+\frac{2n+1}{2}\int_{-\infty}^{\infty}x^{2n}e^{-x^2}\,dx\\
&=\boxed{\left(n+\frac12\right)I_n}.
\end{aligned}
$$

The boundary term vanishes because the Gaussian [exponential function](../../../../../exponential-function.md) decays faster than any fixed power. These [improper integrals](../../../../../improper-integral.md) are absolutely convergent, justifying the limiting [integration by parts](../../../../../integration-by-parts.md).

Starting from the permitted [Gaussian integral](../../../../../gaussian-integral.md) $I_0=\sqrt\pi$, the [Gaussian moment recurrence](../../../../../gaussian-moment-recurrence.md) gives $I_1=\sqrt\pi/2$ and then

$$
\boxed{I_2=\frac34\sqrt\pi,\qquad I_3=\frac{15}{8}\sqrt\pi.}
$$

More generally, iteration gives $I_n=(2n-1)!!\sqrt\pi/2^n$, using the [double factorial](../../../../../double-factorial.md) with $(-1)!!=1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
