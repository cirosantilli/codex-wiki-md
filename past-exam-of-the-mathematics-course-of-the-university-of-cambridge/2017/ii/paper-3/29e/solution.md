<h1 id="29e/solution">Solution</h1>

↑ **Parent:** [29E](../29e.md)

The exponent $\Phi(t)=\tfrac i2(t-t^{-1})$ has saddles $t=\pm i$, with $\Phi(-i)=1$ and $\Phi(i)=-1$. Since the integrand is analytic off the origin, deform the contour to the unit [circle](../../../../../circle.md) and rotate $t=-i e^{i\theta}$. This gives the exact representation

$$
 I_0(x)=\frac1{2\pi}\int_{-\pi}^{\pi}e^{x\cos\theta}\,d\theta.
$$

The dominant saddle at $\theta=0$ is a steepest-descent direction for the [method of steepest descent](../../../../../method-of-steepest-descent.md): $\cos\theta=1-\theta^2/2+\theta^4/24-\cdots$. Set $\theta=s/\sqrt x$ and expand the analytic amplitude against $e^{-s^2/2}$. Integrating its Gaussian moments gives the leading factor $e^x/\sqrt{2\pi x}$; the rest of the contour is exponentially smaller than this dominant contribution outside any fixed neighbourhood of the maximum.

To obtain every coefficient efficiently, the [integral](../../../../../integral.md) satisfies $x^2I_0''+xI_0'-x^2I_0=0$, by differentiating and integrating the [derivative](../../../../../derivative.md) of $\sin\theta\,e^{x\cos\theta}$. Substitute $I_0=e^x x^{-1/2}\sum a_nx^{-n}/\sqrt{2\pi}$ to get $a_0=1$ and $a_n=(2n-1)^2a_{n-1}/(8n)$. Therefore the full [asymptotic expansion](../../../../../asymptotic-expansion.md) is

$$
\boxed{I_0(x)\sim\frac{e^x}{\sqrt{2\pi x}}
 \sum_{n=0}^\infty\frac{((2n-1)!!)^2}{n!\,8^n x^n}
 =\frac{e^x}{\sqrt{2\pi x}}\left(1+\frac1{8x}+\frac9{128x^2}+\frac{225}{3072x^3}+\cdots\right).}
$$

Here $(-1)!!=1$. For each fixed truncation at $n=N$, the relative remainder is $O(x^{-N-1})$ as $x\to+\infty$. The infinite [series](../../../../../series-mathematics.md) is generally divergent, and this all-orders expansion does not purport to resolve exponentially small saddle contributions or their [Stokes phenomenon](../../../../../stokes-phenomenon.md).

## ↑ Ancestors (10)

1. [29E](../29e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
