<h1 id="14a/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Rewrite the ratio of hyperbolic sines as

$$
Y(x,p)=\frac ap\frac{e^{-px/c}-e^{-p(2L-x)/c}}{1-e^{-2pL/c}}.
$$

For $\operatorname{Re}p>0$, expand the denominator by the [geometric series](../../../../../../../geometric-series.md). Part (a) inverts each delayed exponential:

$$
\boxed{y(x,t)=a\sum_{m=0}^\infty\left[H\!\left(t-\frac{2mL+x}{c}\right)-H\!\left(t-\frac{(2m+2)L-x}{c}\right)\right].}
$$

At each finite time only finitely many terms are nonzero, so this [reflected-step solution of the wave equation](../../../../../../../reflected-step-solution-of-the-wave-equation.md) is locally a finite sum. The first front travels from $x=0$; the second is its sign-reversed reflection from the fixed endpoint, with repeated round trips. At $x=L$ the delays coincide and cancel. At $x=0$ the sum telescopes to $a$ for $t>0$.

An equivalent standing-wave [Fourier series](../../../../../../../fourier-series-split.md) is

$$
y(x,t)=a(1-x/L)-\frac{2a}{\pi}\sum_{n=1}^\infty\frac{\sin(n\pi x/L)}n\cos(n\pi ct/L).
$$

Its static ramp has exactly the sine coefficients $2a/(n\pi)$, so cancellation gives the zero initial displacement in the interior. Both representations solve the equation away from the fronts and in the distributional sense across them; the convention $H(0)=1/2$ agrees with Fourier midpoint values.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [14A](../../../14a.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
