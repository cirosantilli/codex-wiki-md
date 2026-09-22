<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under regularity and integrability conditions permitting the limits to pass through the integral, apply the difference quotient directly in time:

$$
\begin{aligned}
\mathcal F_x[u_t](k,t)&=\lim_{h\to0}\int_{\mathbb R}\frac{u(x,t+h)-u(x,t)}h e^{-ikx}dx\\
&=\lim_{h\to0}\frac{\widetilde u(k,t+h)-\widetilde u(k,t)}h=\partial_t\widetilde u(k,t).
\end{aligned}
$$

For the spatial derivative, translate the integration variable in the first term:

$$
\begin{aligned}
\mathcal F_x[u_x](k,t)&=\lim_{h\to0}\int_{\mathbb R}\frac{u(x+h,t)-u(x,t)}h e^{-ikx}dx\\
&=\lim_{h\to0}\frac{e^{ikh}-1}{h}\widetilde u(k,t)=ik\widetilde u(k,t).
\end{aligned}
$$

Consequently

$$
\boxed{\mathcal F_x[u_t]=\partial_t\widetilde u,\qquad\mathcal F_x[u_x]=ik\widetilde u.}
$$

The second calculation is the [Translation property of the Fourier transform](../../../../../translation-property-of-the-fourier-transform.md) applied to a difference quotient. These are the [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) identities. The stated decay removes boundary terms in the alternative integration-by-parts derivation; rigorous interchange of limits also requires suitable control, for example integrable derivatives. The formulas extend to [tempered distributions](../../../../../tempered-distribution.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
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
