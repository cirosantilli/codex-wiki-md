<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $X=\epsilon x$ and suppose $k^2(X)$ stays positive and sufficiently smooth in the region considered. Write $y=\exp[\epsilon^{-1}S_0(X)+S_1(X)+\cdots]$ in $\epsilon^2y_{XX}+k^2(X)y=0$. The leading and first transport equations of the [WKB approximation](../../../../../wkb-approximation.md) are

$$
(S_0')^2+k^2=0,\qquad 2S_0'S_1'+S_0''=0.
$$

With $K=\sqrt{k^2}>0$, they give $S_0'=\pm iK$ and $S_1=-\tfrac12\log K+\text{constant}$. Thus the leading [WKB approximation for a slowly varying oscillator](../../../../../wkb-approximation-for-a-slowly-varying-oscillator.md) is

$$
\boxed{y(x)\sim K(\epsilon x)^{-1/2}\left[C_+e^{i\int^xK(\epsilon s)\,ds}+C_-e^{-i\int^xK(\epsilon s)\,ds}\right].}
$$

The amplitude is fixed by the transport equation, not just by replacing the constant [wave number](../../../../../wavenumber.md) in a sinusoid. The local validity condition is that variation of $K$ over a wavelength is small, for example $|dK/dx|/K^2\ll1$.

If $k^2=-\kappa^2<0$, the same calculation gives the evanescent form

$$
\boxed{y(x)\sim\kappa(\epsilon x)^{-1/2}\left[C_+e^{\int^x\kappa(\epsilon s)\,ds}+C_-e^{-\int^x\kappa(\epsilon s)\,ds}\right].}
$$

At a [classical turning point](../../../../../classical-turning-point.md) where $k^2$ vanishes, these amplitudes diverge and the separated WKB descriptions cease to be uniform. For a simple zero, an [Airy turning-point connection formula](../../../../../airy-turning-point-connection-formula.md) replaces them in an $O(\epsilon^{2/3})$ interval in $X$; it connects oscillation to exponential behavior with the usual quarter-phase shift. A higher-order zero needs a different local canonical problem, so the Airy statement assumes a simple turning point.

For a smooth positive weight $r$ on the closed interval, let $T=\int_0^\pi\sqrt{r(x)}\,dx$. The local [wave number](../../../../../wavenumber.md) in the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) is $\sqrt\lambda\sqrt r$, and the condition at zero selects a sine. Imposing the condition at $\pi$ gives the [WKB quantization condition](../../../../../wkb-quantization-condition.md)

$$
\sqrt{\lambda_n}\,T\sim n\pi,\qquad\boxed{\lambda_n\sim\left(\frac{n\pi}{T}\right)^2,\quad y_n(x)\sim C_n r(x)^{-1/4}\sin\left[\frac{n\pi}{T}\int_0^x\sqrt{r(s)}\,ds\right],\quad n\to\infty.}
$$

For weighted normalization $\int_0^\pi r|y_n|^2dx=1$, rapidly oscillating averaging gives $C_n\sim\sqrt{2/T}$. There is no turning-point phase correction here because $r$ stays positive at both endpoints with [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md).

In the specified example $r(x)=(x+1)^{-2}$, so $T=\log(1+\pi)=L$ and $\lambda_n^{\rm WKB}=(n\pi/L)^2$. To solve exactly, set $t=\log(x+1)$ and $y=\sqrt{x+1}\,w(t)$. Direct differentiation reduces the [Euler-Cauchy equation](../../../../../euler-cauchy-equation.md) to $w''+(\lambda-1/4)w=0$ on $0<t<L$, with zero endpoint values. Hence the [inverse-square weighted Dirichlet spectrum](../../../../../inverse-square-weighted-dirichlet-spectrum.md) is

$$
\boxed{\lambda_n^{\rm exact}=\frac14+\left(\frac{n\pi}{L}\right)^2,\qquad y_n(x)=C_n\sqrt{x+1}\sin\left[\frac{n\pi\log(x+1)}L\right],\quad n=1,2,\ldots.}
$$

Values $\lambda\leq1/4$ give no nonzero solution satisfying both endpoint conditions. The WKB [eigenfunction](../../../../../eigenfunction.md) shape after leading quantization is actually identical to this exact shape; the leading [eigenvalue](../../../../../eigenvalue.md) omits $1/4$.

Using the exact [eigenvalue](../../../../../eigenvalue.md) as the reference, its relative error is

$$
\frac{\lambda_n^{\rm exact}-\lambda_n^{\rm WKB}}{\lambda_n^{\rm exact}}=\frac1{1+4(n\pi/L)^2}<0.01\quad\Longleftrightarrow\quad n>\frac{\sqrt{99}\,L}{2\pi}\simeq2.25.
$$

Thus **$n\geq3$ is sufficient and necessary among positive integers**. Referencing the approximate value instead gives $n>5L/\pi$, and the same integer answer.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
