<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $s=\lambda t>0$. In the [heat-kernel convolution](../../../../../heat-kernel-convolution.md), complete the real square as

$$
\alpha^2y^2+\frac{(x-y)^2}{4s}
=\left(\alpha^2+\frac1{4s}\right)
\left(y-\frac{x}{1+4s\alpha^2}\right)^2
+\frac{\alpha^2x^2}{1+4s\alpha^2}.
$$

The [Gaussian integral](../../../../../gaussian-integral.md) therefore gives

$$
\boxed{\beta=\frac{\alpha}{\sqrt{1+4\lambda t\alpha^2}},\qquad
u(x,t)=\frac{\beta}{\sqrt\pi}e^{-\beta^2x^2}}.
$$

At $t=0$ the same formula gives $\beta=\alpha$. Equivalently, $\beta^{-2}=\alpha^{-2}+4\lambda t$: the [variance](../../../../../variance-split.md) of this normalized [Gaussian function](../../../../../gaussian-function.md) grows from $1/(2\alpha^2)$ to $1/(2\alpha^2)+2\lambda t$.

The initial profiles have unit integral and concentrate at zero as $\alpha\to\infty$. Precisely, for every smooth compactly supported [test function](../../../../../test-function.md) $\varphi$,

$$
\int_{\mathbb R}\frac{\alpha}{\sqrt\pi}e^{-\alpha^2y^2}\varphi(y)\,dy
=\frac1{\sqrt\pi}\int_{\mathbb R}e^{-v^2}\varphi(v/\alpha)\,dv
\longrightarrow\varphi(0).
$$

Thus the limit is the [Dirac delta distribution](../../../../../dirac-delta-function.md), rather than an ordinary function: pointwise the profiles tend to zero away from the origin and diverge at the origin. At every fixed $t>0$,

$$
\boxed{u(\cdot,0)\longrightarrow\delta_0\ \text{in distributions},\qquad
u(x,t)\longrightarrow\frac1{\sqrt{4\pi\lambda t}}e^{-x^2/(4\lambda t)}}.
$$

The limiting evolved profile is the [heat kernel](../../../../../heat-kernel.md) for a unit point source.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
