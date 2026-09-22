<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the cubic denominator as $(\omega-i)(\omega^2+4)$. Substitution gives

$$
\widetilde y(\omega)=\frac{i\omega}{(\omega-i)^2(\omega^2+4)}.
$$

There is a double [pole](../../../../../pole.md) at $i$ and simple poles at $2i,-2i$. For $t>0$, close the inverse-transform contour counterclockwise in the upper half-plane. The [residue](../../../../../residue.md) at the double pole is

$$
\begin{aligned}
\operatorname{Res}_{\omega=i}\big(\widetilde y e^{i\omega t}\big)
&=\left.\frac d{d\omega}\left(\frac{i\omega e^{i\omega t}}{\omega^2+4}\right)\right|_{\omega=i}\\
&=i\left(\frac59-\frac t3\right)e^{-t},
\end{aligned}
$$

and the residue at $2i$ is $-ie^{-2t}/2$. Multiplication by $i$ from the [residue theorem](../../../../../residue-theorem.md) therefore gives $y(t)=(t/3-5/9)e^{-t}+e^{-2t}/2$.

For $t<0$, the clockwise lower closure encloses only $-2i$, with residue $-ie^{2t}/18$. The orientation supplies $-i$, giving $y(t)=-e^{2t}/18$. Hence the continuous solution is

$$
\boxed{y(t)=\begin{cases}-\dfrac1{18}e^{2t},&t<0,\\[2pt]-\dfrac1{18},&t=0,\\[2pt]\left(\dfrac t3-\dfrac59\right)e^{-t}+\dfrac12e^{-2t},&t>0.\end{cases}}
$$

The large inverse-transform arcs vanish: the rational factor is $O(\omega^{-3})$, while the exponential is bounded on the appropriate closure.

<a id="5/c/image-the-two-sided-decaying-fourier-solution-it-and-its-first-derivative-are-continuous-at-zero"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2-2016-ib-fourier-solution.png)

**[Figure 3](#5/c/image-the-two-sided-decaying-fourier-solution-it-and-its-first-derivative-are-continuous-at-zero). The two-sided decaying Fourier solution; it and its first derivative are continuous at zero**.

The graph tends to zero from below as $t\to-\infty$, passes through $y(0)=-1/18$ with slope $-1/9$, reaches a small negative minimum after zero, then crosses the axis, reaches a positive maximum and tends to zero from above. The positive-time stationary points solve $8/9-t/3=e^{-t}$, and the crossing solves $t/3-5/9+e^{-t}/2=0$; these equations determine the sketch without guessing signs.

For a distributional check, $y$ and $y'$ are continuous, while $y''(0^+)-y''(0^-)=1$. The [jump conditions for a third-order Green function](../../../../../jump-conditions-for-a-third-order-green-function.md) therefore produce the delta in $f'=\delta-e^{-t}H(t)$, and each smooth branch satisfies the remaining equation. The nonzero solution for $t<0$ is consistent with the stipulated decay at both temporal infinities. Those are two-sided conditions, not a causality assumption: this is the setting of a [decaying two-sided Green function of a constant-coefficient ordinary differential equation](../../../../../decaying-two-sided-green-function-of-a-constant-coefficient-ordinary-differential-equation.md) and [causality versus stability of a Green function](../../../../../causality-versus-stability-of-a-green-function.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
