<h1 id="14c/solution">Solution</h1>

↑ **Parent:** [14C](../14c.md)

The [convolution](../../../../../convolution.md) is $(f*g)(x)=\int_{-\infty}^{\infty}f(y)g(x-y)\,dy$. Under the usual integrability hypotheses, [Fubini's theorem](../../../../../fubini-s-theorem.md) and $u=x-y$ give

$$
\begin{aligned}
\widetilde{f*g}(k)
&=\iint e^{-ikx}f(y)g(x-y)\,dy\,dx\\
&=\left(\int e^{-iky}f(y)\,dy\right)
\left(\int e^{-iku}g(u)\,du\right)
=\boxed{\widetilde f(k)\widetilde g(k)}.
\end{aligned}
$$

The supplied transform and the [Fourier shift theorem](../../../../../fourier-shift-theorem.md) give

$$
\mathcal F\!\left(\frac{\sin x}{x}\right)
=\begin{cases}\pi,&|k|<1,\\0,&|k|>1.\end{cases}
$$

Since

$$
\frac{\sin x}{x^2}=\frac{\cos x}{x}-\frac d{dx}\left(\frac{\sin x}{x}\right),
$$

the shift and differentiation rules yield

$$
\boxed{
\mathcal F\!\left(\frac{\sin x}{x^2}\right)(k)
=\begin{cases}
-i\pi k,&|k|\leq1,\\
-i\pi\,\operatorname{sgn}k,&|k|\geq1.
\end{cases}}
$$

The coincident boundary values make the endpoint convention immaterial.

## ↑ Ancestors (10)

1. [14C](../14c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
