<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Factor the denominator as $(z^2+1)(z^2+4)$ and integrate

$$
F(z)=\frac{e^{iz}}{(z^2+1)(z^2+4)}
$$

over $[-R,R]$ followed by the upper semicircle, for $R>2$. The enclosed [simple poles](../../../../simple-pole.md) are $i$ and $2i$. The local quotient formula from part (a) gives

$$
\operatorname{Res}_i F=\frac{e^{-1}}{(2i)(3)}=\frac{e^{-1}}{6i},\qquad
\operatorname{Res}_{2i}F=\frac{e^{-2}}{(-3)(4i)}=-\frac{e^{-2}}{12i}.
$$

On this arc, $|e^{iz}|=e^{-\operatorname{Im}z}\leq1$ and $|z^2+1|\geq R^2-1$, $|z^2+4|\geq R^2-4$. Thus the [estimation lemma](../../../../estimation-lemma.md) gives

$$
\left|\int_{\mathrm{arc}}F(z)\,dz\right|\leq\frac{\pi R}{(R^2-1)(R^2-4)}\longrightarrow0.
$$

On the [real line](../../../../real-line.md), $|F(x)|\leq1/[(x^2+1)(x^2+4)]$, so the [improper integral](../../../../improper-integral.md) is absolutely convergent. Hence the [residue theorem](../../../../residue-theorem.md) yields

$$
\int_{-\infty}^{\infty}\frac{e^{ix}}{x^4+5x^2+4}\,dx
=2\pi i\left(\frac{e^{-1}}{6i}-\frac{e^{-2}}{12i}\right).
$$

Taking real parts is justified by absolute convergence. Therefore

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{x^4+5x^2+4}\,dx=\frac\pi{3e}-\frac\pi{6e^2}}.
$$

The imaginary part vanishes as a further check, since the sine integrand is odd.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [5](../../5.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
