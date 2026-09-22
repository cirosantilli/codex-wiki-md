<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Laplace identities.** The one-sided [Laplace transform](../../../../laplace-transform.md) is

$$
\boxed{F(p)=\int_0^\infty e^{-pt}f(t)\,dt,}
$$

for $\operatorname{Re}p$ sufficiently large that the integral converges. For a piecewise smooth [function](../../../../function-split.md) of exponential order, [integration by parts](../../../../integration-by-parts.md) gives

$$
\mathcal L[f'](p)=[e^{-pt}f(t)]_0^\infty+p\int_0^\infty e^{-pt}f(t)\,dt=\boxed{pF(p)-f(0)}.
$$

Differentiating under the [integral](../../../../integral-split.md) gives

$$
F'(p)=-\int_0^\infty t e^{-pt}f(t)\,dt,\qquad\boxed{\mathcal L[tf](p)=-F'(p)}.
$$

Iteration also yields $\mathcal L[f'']=p^2F-pf(0)-f'(0)$. For real $k$ and $p>0$, taking the imaginary part of $(p-ik)^{-1}$ gives

$$
\boxed{\mathcal L[\sin kt](p)=\frac k{p^2+k^2}.}
$$

**Transformed differential equation.** Let $G=\mathcal L[g]$, using the initial values $g(0)=1,g'(0)=0$. Then

$$
\begin{aligned}
\mathcal L[tg'']&=-\frac d{dp}(p^2G-p)=-2pG-p^2G'+1,\\
2\mathcal L[g']&=2pG-2,\\
\alpha^2\mathcal L[tg]&=-\alpha^2G'.
\end{aligned}
$$

Summing the three contributions gives

$$
\boxed{G'(p)=-\frac1{p^2+\alpha^2}.}
$$

For $\alpha\ne0$, the condition $G(p)\to0$ as $p\to\infty$ fixes the integration constant:

$$
G(p)=\int_p^\infty\frac{dq}{q^2+\alpha^2}=\frac1\alpha\arctan\frac\alpha p\qquad(p>0).
$$

It is simpler to invert the derivative: $\mathcal L[tg]=-G'=1/(p^2+\alpha^2)=\mathcal L[\sin(\alpha t)/\alpha]$. Thus

$$
\boxed{g(t)=\frac{\sin(\alpha t)}{\alpha t}\quad(t>0),\qquad g(0)=1.}
$$

This is the [sinc function](../../../../sinc-function.md). Its [Taylor series](../../../../taylor-series.md) begins $1-\alpha^2t^2/6+O(t^4)$, verifying both initial values. For a direct differential check set $h=tg=\sin(\alpha t)/\alpha$. Then $h''+\alpha^2h=tg''+2g'+\alpha^2tg=0$. For $\alpha=0$, take the continuous limit $\boxed{g(t)=1}$, which also follows from $G=1/p$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
